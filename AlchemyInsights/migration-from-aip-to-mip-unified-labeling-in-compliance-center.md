---
title: Migrace z AIP na MIP/sjednocení štítků v centru dodržování předpisů
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674319"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="cd4bd-102">Migrace z AIP na MIP/sjednocení štítků v centru dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="cd4bd-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="cd4bd-103">Pokud chcete migrovat z štítků AIP na jednotné popisky v centru zabezpečení a dodržování předpisů, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="cd4bd-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="cd4bd-104">**Aktivace ochrany z portálu Azure**</span><span class="sxs-lookup"><span data-stu-id="cd4bd-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="cd4bd-105">Pokud jste to ještě neudělali, otevřete nové okno prohlížeče a [Přihlaste se k portálu Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="cd4bd-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="cd4bd-106">Přejděte na zásuvný panel **Azure Information Protection** .</span><span class="sxs-lookup"><span data-stu-id="cd4bd-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="cd4bd-107">Například v nabídce centrum klikněte na **všechny služby** a začněte zadávat **informace** do pole Filtr.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="cd4bd-108">Vyberte možnost **ochrana Azure Information**.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="cd4bd-109">Pokud jste se ještě před tím, než jste předtím nepracovali s doplňkem pro ochranu informací Azure, podívejte se na jednorázový [dodatečný postup](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) přidání tohoto okna na portál.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="cd4bd-110">Pokud chcete otevřít okno Azure Information Protection, musíte mít [plán prémiové ochrany informací pro Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) nebo plán Office 365, který zahrnuje správu přístupových práv.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="cd4bd-111">Pokud máte jedno z těchto předplatných, ale zobrazí se zpráva, že platné předplatné nejde najít, [kontaktujte podporu Microsoftu](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) nebo použijte svůj standardní kanál podpory.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="cd4bd-112">Vyhledejte možnosti **Spravovat** nabídku a vyberte **Aktivace zámku**.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="cd4bd-113">Klikněte na **aktivovat**a potvrďte akci.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="cd4bd-114">Po dokončení aktivace se na informačním panelu zobrazí **Aktivace úspěšně dokončeno**.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="cd4bd-115">**Migrace štítků ochrany informací v Azure do centra zabezpečení Office 365 Security &**</span><span class="sxs-lookup"><span data-stu-id="cd4bd-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="cd4bd-116">Ujistěte se, že jste přihlášeni jako uživatel s oprávněním globálního správce.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="cd4bd-117">Přejděte na zásuvný panel **Azure Information Protection** .</span><span class="sxs-lookup"><span data-stu-id="cd4bd-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="cd4bd-118">V nabídce **Spravovat** vyberte možnost **jednotný popisek**.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="cd4bd-119">V okně pro **ochranu informací v Azure – sjednocení popisků** klikněte na **aktivovat** a postupujte podle online pokynů.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="cd4bd-120">**Poznámka**: Zkontrolujte, jestli máte příslušná oprávnění, a teprve pak & migraci centra dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="cd4bd-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="cd4bd-121">Další informace najdete v těchto článcích:</span><span class="sxs-lookup"><span data-stu-id="cd4bd-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="cd4bd-122">Potřebujete být globálním správcem pro konfiguraci ochrany informací Azure nebo pro delegování jiným správcům?</span><span class="sxs-lookup"><span data-stu-id="cd4bd-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="cd4bd-123">Důležité informace o rolích pro správu po migraci do centra dodržování předpisů &</span><span class="sxs-lookup"><span data-stu-id="cd4bd-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="cd4bd-124">Další informace o AIP pro sjednocení migrace do centra zabezpečení a dodržování předpisů najdete v článku [migrace popisků](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="cd4bd-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
