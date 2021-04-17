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
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrace z programu AIP na mip/unified labeling v Centru dodržování předpisů

Pokud chcete migrovat z popisků AIP do jednotného označování v Centru zabezpečení a dodržování předpisů, proveďte toto:

**Aktivace ochrany z portálu Azure Portal**

1. Pokud jste to ještě neudělali, otevřete nové okno prohlížeče a přihlaste se [na portál Azure Portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Přejděte do okna **Azure Information Protection.** Například v nabídce centrum klikněte  na Všechny služby a začněte psát **informace** do pole Filtr. Vyberte **Azure Information Protection**. Pokud jste se k okně Azure Information Protection ještě [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) předtím nes přístupem, podívejte se na další postup, jak toto okno přidat na portál. Abyste otevřeli okno Azure Information Protection, musíte mít plán [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) nebo plán Office 365, který zahrnuje správu přístupových práv. Pokud máte jedno z těchto předplatných, ale zobrazí se zpráva, že platné předplatné nelze najít, kontaktujte podporu [Microsoftu](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) nebo použijte standardní kanály podpory.

2. Vyhledejte **možnosti nabídky** Spravovat a vyberte **Aktivace ochrany**. Klikněte **na Aktivovat** a potvrďte akci. Po dokončení aktivace se na informačním panelu zobrazí **úspěšně dokončená aktivace.**

**Migrace štítků Azure Information Protection do Centra zabezpečení Office 365 & dodržování předpisů**

1. Ujistěte se, že jste přihlášení jako uživatel s oprávněním globálního správce.

2. Přejděte do okna **Azure Information Protection.**

3. V nabídce **Manage** (Spravovat) vyberte **Unified labeling (Jednotné popisky).**

4. V okně **Azure Information Protection – Jednotné označování** klikněte na **Aktivovat** a postupujte podle pokynů online.

**Poznámka:** Před aktivací migrace Centra zabezpečení & dodržování předpisů ověřte, jestli máte příslušná oprávnění. Další informace najdete v těchto článcích:

1. [Potřebujete být globálním správcem pro konfiguraci Azure Information Protection nebo můžu delegovat na jiné správce?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Důležité informace o rolích správy po migraci do Centra & dodržování předpisů.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Další informace o migraci AIP na Jednotné označování do Centra zabezpečení a dodržování předpisů najdete v tématu [Migrace štítků](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
