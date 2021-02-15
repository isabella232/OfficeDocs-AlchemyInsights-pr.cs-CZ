---
title: Nefunguje zpětný zápis hesla
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243287"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="37c75-102">Nefunguje zpětný zápis hesla</span><span class="sxs-lookup"><span data-stu-id="37c75-102">Password Writeback is not working</span></span>

<span data-ttu-id="37c75-103">**Mám problémy s konfigurací zpětného zápisu hesla**</span><span class="sxs-lookup"><span data-stu-id="37c75-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="37c75-104">Zpětný zápis hesla je prémiová funkce.</span><span class="sxs-lookup"><span data-stu-id="37c75-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="37c75-105">Ujistěte se, že rozumíte licenčním požadavkům:</span><span class="sxs-lookup"><span data-stu-id="37c75-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="37c75-106">Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.</span><span class="sxs-lookup"><span data-stu-id="37c75-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="37c75-107">**Jenom cloudové uživatele** – všechny placené SKU Office 365 (O365) nebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="37c75-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="37c75-108">**Cloudové a místní** uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="37c75-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="37c75-109">Další informace o licenčních požadavcích najdete v článku o licenčních požadavcích pro samoobslužné [resetování hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="37c75-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="37c75-110">Máte aspoň jeden účet správce a jeden zkušební uživatelský účet s jednou z příslušné licence.</span><span class="sxs-lookup"><span data-stu-id="37c75-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="37c75-111">Aby zpětné zapisování hesla fungovalo, musíte Připojit Azure AD Connect k emulátoru primárního řadiče domény.</span><span class="sxs-lookup"><span data-stu-id="37c75-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="37c75-112">Azure AD Connect můžete nakonfigurovat tak, aby bylo  možné používat primární řadič domény, a to tak, že kliknete pravým tlačítkem na vlastnosti konektoru synchronizace služby Active Directory a pak vyberete **konfigurovat oddíly adresáře.**</span><span class="sxs-lookup"><span data-stu-id="37c75-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="37c75-113">Odtud vyhledejte část  nastavení připojení řadičů domén a zaškrtněte políčko s názvem Používají se **jenom preferované řadiče domény.**</span><span class="sxs-lookup"><span data-stu-id="37c75-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="37c75-114">Pokud upřednostňovaný kód DC není emulátoru PDC, Azure AD Connect stále kontaktovat PDC kvůli zpětnému zápisu hesla.</span><span class="sxs-lookup"><span data-stu-id="37c75-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="37c75-115">Resetování hesla je nakonfigurované a povolené ve vašem tenantovi.</span><span class="sxs-lookup"><span data-stu-id="37c75-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="37c75-116">Další informace najdete v článku o tom, [jak uživatelům povolit resetování hesel Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="37c75-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="37c75-117">Ujistěte se, že se účet správce, který se používá k povolení zpětného zápisu hesel, je účet cloudového správce (který se vytvořil v Azure AD ne v místní službě AD).</span><span class="sxs-lookup"><span data-stu-id="37c75-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="37c75-118">Máte místní nasazení AD s jednou nebo více doménovou doménovou doménou, na které běží Windows Server 2008 R2, Windows Server 2012 nebo Windows Server 2012 R2 s nainstalovanými nejnovějšími aktualizacemi Service Pack.</span><span class="sxs-lookup"><span data-stu-id="37c75-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="37c75-119">Máte nainstalovaný nástroj Azure AD Connect a máte připravené prostředí AD pro synchronizaci s cloudem.</span><span class="sxs-lookup"><span data-stu-id="37c75-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="37c75-120">Před testováním zpětného zápisu hesel zkontrolujte, že je v Azure AD Connect nejprve dokončena úplná importovaná a úplná synchronizace ze služby AD i z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37c75-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="37c75-121">Další informace najdete v článku o úplné synchronizaci a [úplném importu v Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="37c75-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="37c75-122">**Mám potíže s připojením k zpětném zápisu hesla**</span><span class="sxs-lookup"><span data-stu-id="37c75-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="37c75-123">Stažení a povolení nejnovější verze [služby Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="37c75-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="37c75-124">Konfigurace brány firewall: Nástroj Azure AD Connect (1.1.443 a vyšší) bude potřebovat **odchozí přístup HTTPS** pro:</span><span class="sxs-lookup"><span data-stu-id="37c75-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="37c75-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="37c75-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="37c75-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="37c75-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="37c75-127">Povolit nečinná připojení, aby se zachovávaly minimálně 2–3 minuty</span><span class="sxs-lookup"><span data-stu-id="37c75-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="37c75-128">**Pořád mám problémy s zpětným zápisem hesla**</span><span class="sxs-lookup"><span data-stu-id="37c75-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="37c75-129">Pokud s tím budou problémy i nadále, zkuste zakázat a znovu povolit službu zpětného zápisu hesel v nástroji Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="37c75-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="37c75-130">Další informace najdete v článku o zakázání a [opětovném povolení zpětného zápisu hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="37c75-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
