---
title: Nelze se přihlásit k Teams kvůli chybě autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038393"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nelze se přihlásit k Teams kvůli chybě autologon.microsoftazuread-sso dot com:443

Pokud je v rámci ověřování O365 povolené bezproblémové jednotné přihlašování, je možné, že bude potřeba adresu URL autologon.microsoftazuread-sso.com přidat na intranetové weby.  Pokud jste ji už dříve přidali k důvěryhodným webům a používáte bezproblémové jednotné přihlašování, měla by být z důvěryhodných webů odebrána.

Podívejte se na [kontrolní seznam pro řešení potíží s bezproblémovým jednotným přihlašováním](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Pokud chcete přidat adresu URL do seznamu intranetových webů, postupujte takto:

1. Spusťte Internet Explorer kliknutím na tlačítko **Start**. Do vyhledávacího pole napište Internet Explorer a pak v seznamu výsledků klikněte na **Internet Explorer**.
2. Klikněte na **Nástroje** a pak na **Možnosti Internetu**.
3. Klikněte na kartu **Zabezpečení**.
4. Teď klikněte na **weby místního intranetu**, klikněte na tlačítko **weby** a pak na tlačítko **Upřesnit**.
5. Zadejte adresu URL webu a klikněte na **Přidat**.
6. Po dokončení klikněte na **Zavřít**.

Další informace najdete v článku o [dokumentaci pro nasazení bezproblémového jednotného přihlašování k Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (obsahuje proces založený na zásadách k přidání adresy URL k intranetovým webům v kroku 3).
