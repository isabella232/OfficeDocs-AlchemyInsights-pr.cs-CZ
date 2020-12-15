---
title: Zařízení čeká na vyřízení.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677572"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="5acbc-102">Zařízení čeká na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="5acbc-102">Device in pending state</span></span>

<span data-ttu-id="5acbc-103">**Požadovaných**</span><span class="sxs-lookup"><span data-stu-id="5acbc-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="5acbc-104">Pokud zadáváte registrace zařízení poprvé, ujistěte se, že jste provedli kontrolu nad [správou zařízení v Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , která vás seznámí s postupem, jak získat zařízení pod kontrolou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5acbc-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="5acbc-105">Pokud zaregistrujete zařízení do Azure AD přímo a zapíšete je do Intune, budete muset zajistit, že jste [nakonfigurovali](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) v Intune, a budete mít nejdřív [licenci](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="5acbc-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="5acbc-106">Zkontrolujte, jestli máte oprávnění provádět operace v Azure AD a místním AD.</span><span class="sxs-lookup"><span data-stu-id="5acbc-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="5acbc-107">Jenom globální správce Azure AD může spravovat nastavení pro registrace zařízení.</span><span class="sxs-lookup"><span data-stu-id="5acbc-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="5acbc-108">Pokud navíc nastavujete automatické registrace v místní službě Active Directory, budete muset být správcem služby Active Directory a AD FS (Pokud je to možné).</span><span class="sxs-lookup"><span data-stu-id="5acbc-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="5acbc-109">Proces registrace hybridního služby Azure AD vyžaduje, aby zařízení byla v podnikové síti.</span><span class="sxs-lookup"><span data-stu-id="5acbc-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="5acbc-110">Funguje to taky přes VPN, ale je to jen to.</span><span class="sxs-lookup"><span data-stu-id="5acbc-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="5acbc-111">Všichni vyslechní zákazníci, kteří potřebují pomoct s odstraňováním potíží se službou hybridního připojení Azure AD v části vzdálené práce.</span><span class="sxs-lookup"><span data-stu-id="5acbc-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="5acbc-112">**Prostředí pro ověřování v cloudu (pomocí algoritmu hash synchronizace nebo předávacího ověřování v Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="5acbc-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="5acbc-113">Tento registrační tok se označuje také jako "synchronizační spojení".</span><span class="sxs-lookup"><span data-stu-id="5acbc-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="5acbc-114">Tady je přehled toho, co se děje během registrace:</span><span class="sxs-lookup"><span data-stu-id="5acbc-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="5acbc-115">Windows 10 vyhledá záznam spojovacího bodu služby, když se uživatel přihlásí do zařízení.</span><span class="sxs-lookup"><span data-stu-id="5acbc-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="5acbc-116">Zařízení se nejprve pokusí načíst informace o tenantovi ze služby SCP na straně klienta v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="5acbc-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="5acbc-117">Další informace najdete v tématu [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="5acbc-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="5acbc-118">Pokud selže, zařízení komunikuje s místní službou Active Directory, aby získala informace o tenantovi ze služby SCP.</span><span class="sxs-lookup"><span data-stu-id="5acbc-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="5acbc-119">Pokud chcete ověřit spojovací bod služby, přečtěte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="5acbc-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="5acbc-120">Doporučujeme, abyste v adresáři Active Directory povolili spojovací bod služby a aby se při počátečním ověřování používaly spojovací bod služby.</span><span class="sxs-lookup"><span data-stu-id="5acbc-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="5acbc-121">Ve Windows 10 se pokoušíte komunikovat s Azure AD v kontextu systému, abyste se ověřili vůči službě Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5acbc-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="5acbc-122">Můžete ověřit, jestli má zařízení přístup k prostředkům společnosti Microsoft pod účtem System pomocí skriptu pro [připojení k testování registrace zařízení](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="5acbc-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="5acbc-123">Windows 10 generuje certifikát podepsaný svým držitelem a uloží ho pod objektem počítače v místním adresáři Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5acbc-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="5acbc-124">To vyžaduje, aby řadič domény promohl.</span><span class="sxs-lookup"><span data-stu-id="5acbc-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="5acbc-125">Objekt zařízení, který má certifikát, se synchronizuje s Azure AD přes Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5acbc-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="5acbc-126">Cyklus synchronizace je ve výchozím nastavení každých 30 minut, ale závisí na konfiguraci služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5acbc-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="5acbc-127">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="5acbc-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="5acbc-128">V této fázi by mělo být v části zařízení na portálu Azure Portal zobrazeno zařízení s předmětem "**čeká**".</span><span class="sxs-lookup"><span data-stu-id="5acbc-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="5acbc-129">Při příštím přihlášení uživatele k Windows 10 bude registrace dokončena.</span><span class="sxs-lookup"><span data-stu-id="5acbc-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5acbc-130">Pokud používáte připojení k síti VPN, může být aktivace aktivována ručně a odhlášením nebo přihlášením ukončuje připojení domény.</span><span class="sxs-lookup"><span data-stu-id="5acbc-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="5acbc-131">Postup:</span><span class="sxs-lookup"><span data-stu-id="5acbc-131">To do that:</span></span>
    >
    > <span data-ttu-id="5acbc-132">Dejte mu na `dsregcmd /join` počítači lokálně výzvu nebo vzdáleně přes PsExec.</span><span class="sxs-lookup"><span data-stu-id="5acbc-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="5acbc-133">Například: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="5acbc-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="5acbc-134">Běžné problémy s registrací zařízení Azure Active Directory najdete v tématu [Časté otázky k zařízení](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="5acbc-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
