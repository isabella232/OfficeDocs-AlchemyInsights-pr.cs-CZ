---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695316"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Oprava aplikací Microsoft 365 je líto, ale jiný účet z vaší organizace už je přihlášený.

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Pomocí nastavení Windows > **přístup do práce nebo do školy**odeberte všechny pracovní účty s výjimkou příslušného účtu.
- Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0. (Např.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otevřete aplikaci Office **a zvolte**  >  **Account**  >  **Odhlásit**se. Potom se přihlaste pomocí uživatelského účtu s platnou licencí. Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V případě Macu si projděte téma [Nejde se přihlásit k aplikaci Office 2016 pro Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Další informace najdete v tématu ["je nám líto, ale jiný účet z vaší organizace už je přihlášený" v Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).