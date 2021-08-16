---
title: Problémy s přihlášením k Microsoft 365 aplikacím
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028033"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Oprava Microsoft 365 aplikace "Omlouváme se, že už je přihlášený jiný účet z vaší organizace".

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Odeberte všechny pracovní účty kromě ovlivněného účtu pomocí Windows Nastavení > **Accessu v práci nebo ve škole**.
- [Vymažte Office přihlašovací údaje](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Správce přihlašovacích údajů.<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otevřete aplikace Office, zvolte   >  **Souborový**  >  **účet Odhlásit** se . Potom se přihlaste pomocí uživatelského účtu s platnou licencí. Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V případě Macu si projděte téma [Nejde se přihlásit k aplikaci Office 2016 pro Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Další informace najdete v tématu [Omlouváme se,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)ale jiný účet z vaší organizace už je na tomto počítači přihlášený, Office .