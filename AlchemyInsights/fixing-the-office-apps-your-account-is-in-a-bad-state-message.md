---
title: Oprava Microsoft 365 aplikací Váš účet je ve špatném stavu
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
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068229"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Oprava chyby Microsoft 365 "Váš účet je ve špatném stavu".

Pokud chcete tuto chybu vyřešit, vyzkoušejte na příslušném počítači následující možnosti:

- Otevřete aplikace Office, vyberte **Odhlásit** se od účtu souboru  >    >  **ze všech účtů**. Přihlaste se znovu pomocí uživatelského účtu s platnou licencí. Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Vymažte Office přihlašovací údaje](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Správce přihlašovacích údajů.<br>
  **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. Například \Software\Microsoft\Office\16.0\Common\Identity\
- Pokud k chybě dojde při připojování Office 365 pomocí Office 2013, [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) povolte moderní ověřování Office klienta.

Další informace najdete v článku Řešení potíží s aplikacemi mimo prohlížeč, které se neschytá přihlásit k [Microsoftu 365, Azure](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)nebo Intune.

