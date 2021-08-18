---
title: Řešení běžných problémů s Microsoft Defenderem pro Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330053"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Řešení běžných problémů s Microsoft Defenderem pro Office 365

Tady je několik řešení běžných problémů s Microsoft Defenderem pro Office 365:

- **Zpoždění zprávy:**

  Zpoždění při doručování e-mailů může být příčinou Sejf kontroly zpráv v přílohách. Další informace najdete v tématu [Sejf nastavení zásad Přílohy](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Nahlášení falešně pozitivních nebo záporných výsledků:**

  Další informace najdete v tématu [Nahlášení zpráv a souborů do Microsoftu](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Povolení Sejf ochrany odkazů:**

  1. Na portálu Microsoft 365 Defender na webu přejděte na <https://security.microsoft.com/> **E-mail & zásady** spolupráce & pravidla zásady hrozeb Sejf odkazy v \>  \>  \>  **části** Zásady.

     Pokud chcete přejít přímo na **Sejf odkazy,** použijte <https://security.microsoft.com/safelinksv2> .

  2. Na **Sejf odkazy** vyberte zásadu kliknutím na název zásady.
  3. V plovoucím seznamu podrobností, který se zobrazí, proveďte některý z následujících kroků:
     - Pokud chcete přidat novou zásadu, vyberte **+ Vytvořit**. Spustí se průvodce, který vám pomůže definovat nastavení zásad.
     - Pokud chcete upravit existující zásadu, vyberte ji kliknutím na název zásady. V plovoucím seznamu podrobností, který se zobrazí, **vyberte Upravit** v **části Nastavení** ochrany.
  4. Na stránce **Nastavení ochrany** nakonfigurujte následující nastavení:
     - Zapněte možnost **Vybrat akci pro neznámé potenciálně** škodlivé adresy URL ve zprávách .
     - Vyberte **Použít bezpečné odkazy na zprávy odeslané v organizaci**.

  Další informace najdete v tématu Nastavení zásad Sejf odkazy v [programu Microsoft Defender pro Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
