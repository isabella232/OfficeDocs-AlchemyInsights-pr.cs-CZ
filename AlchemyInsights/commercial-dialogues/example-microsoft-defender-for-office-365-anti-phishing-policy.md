---
title: Příklad microsoft defenderu pro Office 365 anti-phishing
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034999"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Příklad microsoft defenderu pro Office 365 anti-phishing

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
