---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579930"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Oprava zprávy Aplikace Microsoft 365 "Omlouváme se, jiný účet z vaší organizace je již přihlášen"

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Odeberte všechny pracovní účty kromě ovlivněného účtu pomocí nastavení Windows > **práce nebo školy aplikace Access**.
- [Vymazání přihlašovacích údajů Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce pověření systému Windows<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otevřete aplikaci Office a zvolte **Odhlásit se**  >  **na účet**souborů  >  **Sign Out**. Pak se přihlaste pomocí uživatelského účtu s platnou licencí. Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V případě Macu si projděte téma [Nejde se přihlásit k aplikaci Office 2016 pro Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Další informace naleznete [v tématu "Omlouváme se, jiný účet z vaší organizace je již přihlášen k tomuto počítači" v office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).