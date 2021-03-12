---
title: Příklad zásad ochrany proti phishingu v Microsoft Defenderu pro Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744896"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Příklad zásad ochrany proti phishingu v Microsoft Defenderu pro Office 365

Tato nastavení povolte zásadu s názvem Doména a *výkonný ředitel*. Tato zásada poskytuje ochranu uživatelů i domén před zosobněním a pak platí pro všechny e-maily přijaté uživateli v doméně. Nejdřív přidejte následující informace k vytvoření zásady:

- **Název:** Domain and CEO **Description**(Popis domény a generálního ředitele): Ujistěte se, že se výkonný ředitel a vaše doména nezosobní.
  **Platí pro:** Vyberte **Doména příjemce je**. V **části Kterýkoli z těchto** možností vyberte **Zvolit** a pak vyberte doménu. Vyberte **+ Přidat**. Zaškrtněte políčko vedle názvu domény v seznamu (například contoso.com *)* a pak vyberte **Přidat**. Vyberte **Hotovo**.
- Po vytvoření zásady můžete zásadu doladit pomocí následujících možností:
  - **Přidání uživatelů k ochraně:** V tomto příkladu přidejte minimálně e-mailovou adresu generálního ředitele.
  - **Přidání domén k ochraně:** Přidejte doménu organizace, která zahrnuje kancelář generálního ředitele.
  - **Zvolte akce:** Pokud  **e-mail** posílá zosobněný uživatel, vyberte Přesměrovat zprávu na jinou *e-mailovou* adresu a zadejte e-mailovou adresu správce zabezpečení (například securityadmin@contoso.com). V **případě, že e-mail odesílá zosobněná doména,** vyberte **Karanténa zprávy**.
  - **Inteligence poštovní** schránky: Ve výchozím nastavení je tato možnost vybraná při vytváření nové zásady ochrany proti phishing. Nejlepších výsledků **dosáhnete, když** toto nastavení necháte na.
  - **Přidání důvěryhodných odesílatelů a domén:** V tomto příkladu nedefinujte žádné přepsání.
- Po prošetřování nastavení vyberte Podle potřeby **možnost** Vytvořit tuto zásadu nebo Uložit.

Další informace najdete v tématu [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
