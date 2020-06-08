---
title: Migrace z AIP na MIP/Jednotné označování v Centru dodržování předpisů
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236361"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="d046e-102">Migrace z AIP na MIP/Jednotné označování v Centru dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="d046e-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="d046e-103">Chcete-li migrovat z popisků AIP do sjednoceného označování v Centru zabezpečení a dodržování předpisů, udělejte toto:</span><span class="sxs-lookup"><span data-stu-id="d046e-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="d046e-104">**Aktivace ochrany z portálu Azure**</span><span class="sxs-lookup"><span data-stu-id="d046e-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="d046e-105">Pokud jste tak ještě neučinili, otevřete nové okno prohlížeče a [přihlaste se k webu Azure Portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d046e-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="d046e-106">Přejděte do okna **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="d046e-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="d046e-107">Například v nabídce centra klikněte na **Všechny služby** a začněte psát **informace** do pole Filtr.</span><span class="sxs-lookup"><span data-stu-id="d046e-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="d046e-108">Vyberte **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="d046e-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="d046e-109">Pokud jste dosud nepřistupovali k okně Azure Information Protection, přečtěte si jednorázové [další kroky](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) k přidání tohoto okna na portál.</span><span class="sxs-lookup"><span data-stu-id="d046e-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="d046e-110">Pokud chcete otevřít okno Azure Information Protection, musíte mít buď [plán Azure Information Protection Premium,](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) nebo plán Office 365, který zahrnuje správu práv.</span><span class="sxs-lookup"><span data-stu-id="d046e-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="d046e-111">Pokud máte jedno z těchto předplatných, ale zobrazí se zpráva, že platné předplatné nelze najít, [obraťte se](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) na podporu společnosti Microsoft nebo použijte standardní kanály podpory.</span><span class="sxs-lookup"><span data-stu-id="d046e-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="d046e-112">Vyhledejte možnosti nabídky **Spravovat** a vyberte **Možnost Aktivace ochrany**.</span><span class="sxs-lookup"><span data-stu-id="d046e-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="d046e-113">Klikněte na **Aktivovat**a potom akci potvrďte.</span><span class="sxs-lookup"><span data-stu-id="d046e-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="d046e-114">Po dokončení aktivace se na informačním panelu zobrazí **aktivace úspěšně dokončená**.</span><span class="sxs-lookup"><span data-stu-id="d046e-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="d046e-115">**Migrace štítků ochrany informací Azure do Centra dodržování zabezpečení Office 365 &**</span><span class="sxs-lookup"><span data-stu-id="d046e-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="d046e-116">Ujistěte se, že jste přihlášeni jako uživatel s oprávněním globálního správce.</span><span class="sxs-lookup"><span data-stu-id="d046e-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="d046e-117">Přejděte do okna **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="d046e-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="d046e-118">V nabídce **Spravovat** vyberte **možnost Jednotné popisování**.</span><span class="sxs-lookup"><span data-stu-id="d046e-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="d046e-119">V **okně Azure Information Protection – jednotné označení** klikněte na **Aktivovat** a postupujte podle pokynů online.</span><span class="sxs-lookup"><span data-stu-id="d046e-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="d046e-120">**Poznámka:** Před aktivací migrace Centra zabezpečení & compliance ověřte, zda máte příslušná oprávnění.</span><span class="sxs-lookup"><span data-stu-id="d046e-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="d046e-121">Další informace najdete v těchto článcích:</span><span class="sxs-lookup"><span data-stu-id="d046e-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="d046e-122">Musíte být globální správce pro konfiguraci Azure Information Protection, nebo mohu delegovat na jiné správce?</span><span class="sxs-lookup"><span data-stu-id="d046e-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="d046e-123">Důležité informace o rolích pro správu po migraci do Centra pro & dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="d046e-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="d046e-124">Další informace o migraci a migraci jednotného popisku AIP do Centra zabezpečení a dodržování předpisů naleznete v [tématu Migrace štítků](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="d046e-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
