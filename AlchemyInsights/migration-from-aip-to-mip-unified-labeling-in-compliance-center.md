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
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrace z AIP na MIP/Jednotné označování v Centru dodržování předpisů

Chcete-li migrovat z popisků AIP do sjednoceného označování v Centru zabezpečení a dodržování předpisů, udělejte toto:

**Aktivace ochrany z portálu Azure**

1. Pokud jste tak ještě neučinili, otevřete nové okno prohlížeče a [přihlaste se k webu Azure Portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Přejděte do okna **Azure Information Protection.** Například v nabídce centra klikněte na **Všechny služby** a začněte psát **informace** do pole Filtr. Vyberte **Azure Information Protection**. Pokud jste dosud nepřistupovali k okně Azure Information Protection, přečtěte si jednorázové [další kroky](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) k přidání tohoto okna na portál. Pokud chcete otevřít okno Azure Information Protection, musíte mít buď [plán Azure Information Protection Premium,](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) nebo plán Office 365, který zahrnuje správu práv. Pokud máte jedno z těchto předplatných, ale zobrazí se zpráva, že platné předplatné nelze najít, [obraťte se](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) na podporu společnosti Microsoft nebo použijte standardní kanály podpory.

2. Vyhledejte možnosti nabídky **Spravovat** a vyberte **Možnost Aktivace ochrany**. Klikněte na **Aktivovat**a potom akci potvrďte. Po dokončení aktivace se na informačním panelu zobrazí **aktivace úspěšně dokončená**.

**Migrace štítků ochrany informací Azure do Centra dodržování zabezpečení Office 365 &**

1. Ujistěte se, že jste přihlášeni jako uživatel s oprávněním globálního správce.

2. Přejděte do okna **Azure Information Protection.**

3. V nabídce **Spravovat** vyberte **možnost Jednotné popisování**.

4. V **okně Azure Information Protection – jednotné označení** klikněte na **Aktivovat** a postupujte podle pokynů online.

**Poznámka:** Před aktivací migrace Centra zabezpečení & compliance ověřte, zda máte příslušná oprávnění. Další informace najdete v těchto článcích:

1. [Musíte být globální správce pro konfiguraci Azure Information Protection, nebo mohu delegovat na jiné správce?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Důležité informace o rolích pro správu po migraci do Centra pro & dodržování předpisů.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Další informace o migraci a migraci jednotného popisku AIP do Centra zabezpečení a dodržování předpisů naleznete v [tématu Migrace štítků](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
