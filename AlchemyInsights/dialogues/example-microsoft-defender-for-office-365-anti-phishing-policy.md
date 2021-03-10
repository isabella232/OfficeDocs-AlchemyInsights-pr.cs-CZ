---
title: Příklad anti-phishingové zásady Microsoft Defenderu pro Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693240"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Příklad anti-phishingové zásady Microsoft Defenderu pro Office 365

Toto nastavení umožňuje zásady s názvem Doména a *generálního ředitele.* Tato zásada poskytuje ochranu před zosobněním uživatele i domény a pak je použije pro všechny e-maily přijaté uživateli v doméně. Nejdřív přidejte následující informace k vytvoření zásady:

- **Název:** Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.
  **Platí pro:** Vyberte **doménu příjemce.** V **části Libovolná z těchto** možností vyberte **Možnost** a pak vyberte doménu. Vyberte **+ Přidat.** Zaškrtněte políčko vedle názvu domény v seznamu (například contoso.com *)* a pak vyberte **Přidat.** Vyberte **Hotovo.**
- Po vytvoření zásady můžete zásadu vyladit pomocí následujících možností:
  - **Ochrana přidáním uživatelů:** V tomto příkladu přidejte minimálně e-mailovou adresu generálního ředitele.
  - **Přidání domén pro ochranu:** Přidejte doménu organizace, která obsahuje kancelář generálního ředitele.
  - **Zvolte akce:** **Pokud** e-mail posílá uživatel zosobněného uživatele, vyberte Přesměrovat zprávu na jinou e-mailovou adresu a potom zadejte e-mailovou adresu správce zabezpečení (například *securityadmin@contoso.com).* Pokud **e-mail posíláte zosobněná doména,** vyberte **Přesunout zprávu do karantény.**
  - **Inteligentní poštovní** schránka: Ve výchozím nastavení je tato možnost vybraná, když vytváříte novou anti-phishingovou zásadu. Nejlepších výsledků **dosáhnete,** když toto nastavení necháte zas.
  - **Přidání důvěryhodných odesílatelů** a domén: V tomto příkladu nedefinujte žádné přepsání.
- Až nastavení prošetříte, vyberte Podle potřeby Vytvořit tuto zásadu nebo **Uložit.** 

Další informace najdete v [anti-phishingových zásadách v Microsoftu 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
