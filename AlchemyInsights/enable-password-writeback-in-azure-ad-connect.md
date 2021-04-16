---
title: Povolení zpětného zápisu hesla v Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814005"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="8e430-102">Povolení zpětného zápisu hesla v Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="8e430-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="8e430-103">Pokud chcete povolit samoobslužný zpětný zápis pro resetování hesla, povolte nejdřív možnost zpětného zápisu v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8e430-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="8e430-104">Na serveru Azure AD Connect proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="8e430-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="8e430-105">Přihlaste se k serveru Azure AD Connect a spusťte průvodce konfigurací **Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="8e430-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="8e430-106">Na úvodní **stránce** klikněte na **Konfigurovat.**</span><span class="sxs-lookup"><span data-stu-id="8e430-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="8e430-107">Na stránce **Další úkoly** vyberte Přizpůsobit **možnosti synchronizace** a potom klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="8e430-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="8e430-108">Na stránce **Připojit se k Azure AD** zadejte přihlašovací údaje globálního správce pro vašeho tenanta Azure a klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="8e430-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="8e430-109">Na **stránkách Propojte adresáře** a **filtrování domény/OU** klikněte na **Další.**</span><span class="sxs-lookup"><span data-stu-id="8e430-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="8e430-110">Na stránce **Volitelné** funkce zaškrtněte políčko vedle položky Zpětný zápis hesla a **klikněte** na **Další.**</span><span class="sxs-lookup"><span data-stu-id="8e430-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="8e430-111">Na stránce **Ready to configure** (Připraveno ke konfiguraci) klikněte na **Configure** (Konfigurovat) a počkejte na dokončení procesu.</span><span class="sxs-lookup"><span data-stu-id="8e430-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="8e430-112">Až uvidíte dokončení konfigurace, klikněte na **Ukončit.**</span><span class="sxs-lookup"><span data-stu-id="8e430-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="8e430-113">S povoleným zpětným zápisem hesel v Azure AD Connect nakonfigurujte Azure AD SSPR pro zpětný zápis.</span><span class="sxs-lookup"><span data-stu-id="8e430-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="8e430-114">Pokud chcete povolit zpětný zápis hesel v SSPR, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="8e430-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="8e430-115">Přihlaste se k webu Azure Portal pomocí účtu globálního správce.</span><span class="sxs-lookup"><span data-stu-id="8e430-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="8e430-116">Vyhledejte a vyberte **Azure Active Directory,** klikněte na **Resetování hesla** a potom klikněte na Místní **integrace.**</span><span class="sxs-lookup"><span data-stu-id="8e430-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="8e430-117">Nastavte možnost Pro zápis hesel zpět do místního **adresáře?** na **Ano**.</span><span class="sxs-lookup"><span data-stu-id="8e430-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="8e430-118">Nastavte možnost Povolit **uživatelům odemknout účty bez resetování hesla?** na **Ano**.</span><span class="sxs-lookup"><span data-stu-id="8e430-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="8e430-119">Až budete připravení, klikněte na **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="8e430-119">When ready, click **Save**.</span></span>

<span data-ttu-id="8e430-120">Další informace najdete v tématu [Povolení samoobslužných](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)zpětných zápisů resetování hesla v Azure Active Directory do místního prostředí .</span><span class="sxs-lookup"><span data-stu-id="8e430-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="8e430-121">Když správce resetuje heslo uživatele na portálu Azure Portal, pokud je tento uživatel federovaný nebo se synchronizuje hodnota hash hesla, heslo se zapisuje zpátky do místního prostředí.</span><span class="sxs-lookup"><span data-stu-id="8e430-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="8e430-122">Tato funkce vyžaduje licenci Azure Premium (P1 nebo P2) a momentálně není podporovaná na portálu pro správu Office.</span><span class="sxs-lookup"><span data-stu-id="8e430-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
