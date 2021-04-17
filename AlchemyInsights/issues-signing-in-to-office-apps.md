---
title: Problémy s přihlášením k aplikacím Microsoft 365
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
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833068"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Oprava zpráv aplikace Microsoft 365 "Omlouváme se, ale už je přihlášený jiný účet z vaší organizace".

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Odeberte všechny pracovní účty kromě ovlivněného účtu pomocí nastavení Windows > **Accessu v práci nebo ve škole**.
- [Vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce přihlašovacích údajů systému Windows.<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otevřete aplikaci Office a zvolte  >  **Souborový účet**  >  **Odhlásit se**. Potom se přihlaste pomocí uživatelského účtu s platnou licencí. Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V případě Macu si projděte téma [Nejde se přihlásit k aplikaci Office 2016 pro Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Další informace najdete v tématu [Omlouváme se,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)ale jiný účet z vaší organizace už je na tomto počítači přihlášený.