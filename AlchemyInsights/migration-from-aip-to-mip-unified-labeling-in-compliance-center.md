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
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrace z AIP na MIP/sjednocení štítků v centru dodržování předpisů

Pokud chcete migrovat z štítků AIP na jednotné popisky v centru zabezpečení a dodržování předpisů, postupujte takto:

**Aktivace ochrany z portálu Azure**

1. Pokud jste to ještě neudělali, otevřete nové okno prohlížeče a [Přihlaste se k portálu Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Přejděte na zásuvný panel **Azure Information Protection** . Například v nabídce centrum klikněte na **všechny služby** a začněte zadávat **informace** do pole Filtr. Vyberte možnost **ochrana Azure Information**. Pokud jste se ještě před tím, než jste předtím nepracovali s doplňkem pro ochranu informací Azure, podívejte se na jednorázový [dodatečný postup](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) přidání tohoto okna na portál. Pokud chcete otevřít okno Azure Information Protection, musíte mít [plán prémiové ochrany informací pro Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) nebo plán Office 365, který zahrnuje správu přístupových práv. Pokud máte jedno z těchto předplatných, ale zobrazí se zpráva, že platné předplatné nejde najít, [kontaktujte podporu Microsoftu](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) nebo použijte svůj standardní kanál podpory.

2. Vyhledejte možnosti **Spravovat** nabídku a vyberte **Aktivace zámku**. Klikněte na **aktivovat**a potvrďte akci. Po dokončení aktivace se na informačním panelu zobrazí **Aktivace úspěšně dokončeno**.

**Migrace štítků ochrany informací v Azure do centra zabezpečení Office 365 Security &**

1. Ujistěte se, že jste přihlášeni jako uživatel s oprávněním globálního správce.

2. Přejděte na zásuvný panel **Azure Information Protection** .

3. V nabídce **Spravovat** vyberte možnost **jednotný popisek**.

4. V okně pro **ochranu informací v Azure – sjednocení popisků** klikněte na **aktivovat** a postupujte podle online pokynů.

**Poznámka**: Zkontrolujte, jestli máte příslušná oprávnění, a teprve pak & migraci centra dodržování předpisů. Další informace najdete v těchto článcích:

1. [Potřebujete být globálním správcem pro konfiguraci ochrany informací Azure nebo pro delegování jiným správcům?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Důležité informace o rolích pro správu po migraci do centra dodržování předpisů &](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Další informace o AIP pro sjednocení migrace do centra zabezpečení a dodržování předpisů najdete v článku [migrace popisků](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
