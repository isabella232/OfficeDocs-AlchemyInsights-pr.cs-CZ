---
title: Poradce při potížích s PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573379"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="41023-102">Poradce při potížích s PRT</span><span class="sxs-lookup"><span data-stu-id="41023-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="41023-103">Aby jakékoli zařízení mohlo dokončit získání ověření, musí být plně registrováno a v dobrém stavu a může získat primární obnovovací token (PRT).</span><span class="sxs-lookup"><span data-stu-id="41023-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="41023-104">Proces registrace hybridního služby Azure AD vyžaduje, aby zařízení byla v podnikové síti.</span><span class="sxs-lookup"><span data-stu-id="41023-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="41023-105">Funguje to taky přes VPN, ale je to jen to.</span><span class="sxs-lookup"><span data-stu-id="41023-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="41023-106">Podíváme se, že zákazníci potřebují pomoct s odstraňováním potíží se službou hybridního připojení Azure AD v rámci podmínek vzdálené práce.</span><span class="sxs-lookup"><span data-stu-id="41023-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="41023-107">Tady je přehled toho, co se děje "pod digestoří" během procesu registrace.</span><span class="sxs-lookup"><span data-stu-id="41023-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="41023-108">**Prostředí pro ověřování v cloudu (pomocí algoritmu hash synchronizace nebo předávacího ověřování v Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="41023-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="41023-109">Tento registrační tok se označuje také jako "synchronizační spojení".</span><span class="sxs-lookup"><span data-stu-id="41023-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="41023-110">Windows 10 zjistí záznam SCP na přihlášení uživatele k zařízení.</span><span class="sxs-lookup"><span data-stu-id="41023-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="41023-111">Zařízení se nejprve pokusí načíst informace o tenantovi ze služby SCP na straně klienta v registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="41023-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="41023-112">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="41023-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="41023-113">Pokud selže, zařízení komunikuje se službou místní služby Active Directory (AD), aby získala informace o tenantovi od spojovacího bodu služby (SCP).</span><span class="sxs-lookup"><span data-stu-id="41023-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="41023-114">Pokud chcete ověřit spojovací bod služby, podívejte se na tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="41023-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="41023-115">Doporučujeme v reklamě povolit spojovací bod služby a k počátečnímu ověření jenom používat spojovací bod služby.</span><span class="sxs-lookup"><span data-stu-id="41023-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="41023-116">Ve Windows 10 se pokoušíte komunikovat s Azure AD v kontextu systému, abyste se ověřili vůči službě Azure AD.</span><span class="sxs-lookup"><span data-stu-id="41023-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="41023-117">Můžete ověřit, jestli má zařízení přístup k prostředkům společnosti Microsoft pod účtem System pomocí skriptu pro připojení k testování registrace zařízení.</span><span class="sxs-lookup"><span data-stu-id="41023-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="41023-118">Windows 10 generuje certifikát podepsaný svým držitelem a uloží ho pod objektem počítače v místním AD.</span><span class="sxs-lookup"><span data-stu-id="41023-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="41023-119">To vyžaduje, aby řadič domény promohl.</span><span class="sxs-lookup"><span data-stu-id="41023-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="41023-120">Objekt zařízení, který má certifikát, se synchronizuje s Azure AD přes Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="41023-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="41023-121">Cyklus synchronizace je ve výchozím nastavení každých 30 minut, ale závisí na konfiguraci služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="41023-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="41023-122">Další informace najdete v tomto [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="41023-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="41023-123">V této fázi by mělo být v části zařízení na portálu Azure Portal zobrazeno zařízení s předmětem "čeká".</span><span class="sxs-lookup"><span data-stu-id="41023-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="41023-124">Při příštím přihlášení uživatele k Windows 10 bude registrace dokončena.</span><span class="sxs-lookup"><span data-stu-id="41023-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="41023-125">Pokud používáte připojení k síti VPN a proces přihlašování se odhlášením ukončí připojení k doméně, můžete ručně spustit registraci:</span><span class="sxs-lookup"><span data-stu-id="41023-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="41023-126">Dejte dsregcmd/JOIN místně ve výzvě pro správu nebo vzdáleně přes PSExec na PC.</span><span class="sxs-lookup"><span data-stu-id="41023-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="41023-127">Například PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="41023-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="41023-128">Další informace o problémech s hybridním připojením najdete v článku [řešení potíží se zařízeními](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="41023-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
