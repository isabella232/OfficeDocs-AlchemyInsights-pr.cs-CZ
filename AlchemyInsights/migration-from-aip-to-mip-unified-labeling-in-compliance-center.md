---
title: Migrace z programu AIP na mip/unified labeling v Centru dodržování předpisů
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825364"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="98b73-102">Migrace z programu AIP na mip/unified labeling v Centru dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="98b73-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="98b73-103">Pokud chcete migrovat z popisků AIP do jednotného označování v Centru zabezpečení a dodržování předpisů, proveďte toto:</span><span class="sxs-lookup"><span data-stu-id="98b73-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="98b73-104">**Aktivace ochrany z portálu Azure Portal**</span><span class="sxs-lookup"><span data-stu-id="98b73-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="98b73-105">Pokud jste to ještě neudělali, otevřete nové okno prohlížeče a přihlaste se [na portál Azure Portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="98b73-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="98b73-106">Přejděte do okna **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="98b73-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="98b73-107">Například v nabídce centrum klikněte  na Všechny služby a začněte psát **informace** do pole Filtr.</span><span class="sxs-lookup"><span data-stu-id="98b73-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="98b73-108">Vyberte **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="98b73-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="98b73-109">Pokud jste se k okně Azure Information Protection ještě [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) předtím nes přístupem, podívejte se na další postup, jak toto okno přidat na portál.</span><span class="sxs-lookup"><span data-stu-id="98b73-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="98b73-110">Abyste otevřeli okno Azure Information Protection, musíte mít plán [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) nebo plán Office 365, který zahrnuje správu přístupových práv.</span><span class="sxs-lookup"><span data-stu-id="98b73-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="98b73-111">Pokud máte jedno z těchto předplatných, ale zobrazí se zpráva, že platné předplatné nelze najít, kontaktujte podporu [Microsoftu](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) nebo použijte standardní kanály podpory.</span><span class="sxs-lookup"><span data-stu-id="98b73-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="98b73-112">Vyhledejte **možnosti nabídky** Spravovat a vyberte **Aktivace ochrany**.</span><span class="sxs-lookup"><span data-stu-id="98b73-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="98b73-113">Klikněte **na Aktivovat** a potvrďte akci.</span><span class="sxs-lookup"><span data-stu-id="98b73-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="98b73-114">Po dokončení aktivace se na informačním panelu zobrazí **úspěšně dokončená aktivace.**</span><span class="sxs-lookup"><span data-stu-id="98b73-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="98b73-115">**Migrace štítků Azure Information Protection do Centra zabezpečení Office 365 & dodržování předpisů**</span><span class="sxs-lookup"><span data-stu-id="98b73-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="98b73-116">Ujistěte se, že jste přihlášení jako uživatel s oprávněním globálního správce.</span><span class="sxs-lookup"><span data-stu-id="98b73-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="98b73-117">Přejděte do okna **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="98b73-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="98b73-118">V nabídce **Manage** (Spravovat) vyberte **Unified labeling (Jednotné popisky).**</span><span class="sxs-lookup"><span data-stu-id="98b73-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="98b73-119">V okně **Azure Information Protection – Jednotné označování** klikněte na **Aktivovat** a postupujte podle pokynů online.</span><span class="sxs-lookup"><span data-stu-id="98b73-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="98b73-120">**Poznámka:** Před aktivací migrace Centra zabezpečení & dodržování předpisů ověřte, jestli máte příslušná oprávnění.</span><span class="sxs-lookup"><span data-stu-id="98b73-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="98b73-121">Další informace najdete v těchto článcích:</span><span class="sxs-lookup"><span data-stu-id="98b73-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="98b73-122">Potřebujete být globálním správcem pro konfiguraci Azure Information Protection nebo můžu delegovat na jiné správce?</span><span class="sxs-lookup"><span data-stu-id="98b73-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="98b73-123">Důležité informace o rolích správy po migraci do Centra & dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="98b73-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="98b73-124">Další informace o migraci AIP na Jednotné označování do Centra zabezpečení a dodržování předpisů najdete v tématu [Migrace štítků](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="98b73-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
