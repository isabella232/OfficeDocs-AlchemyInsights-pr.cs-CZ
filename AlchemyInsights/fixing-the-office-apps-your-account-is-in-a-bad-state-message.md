---
title: Oprava aplikací Microsoft 365, na které je váš účet chybný stav
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744538"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Oprava aplikací Microsoft 365 "váš účet je ve špatném stavu"

Pokud chcete chybu opravit, vyzkoušejte v příslušném počítači následující možnosti:

- Otevřete aplikaci Office a vyberte **soubor**  >  **Account**  >  **Odhlásit se ze všech účtů**. Přihlaste se znovu pomocí uživatelského účtu s platnou licencí. Podrobné informace najdete v článku [Účty v Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br>
  **Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0. Například \Software\Microsoft\Office\16.0\Common\Identity\
- Pokud dojde k chybě při připojování k Office 365 pomocí Office 2013, [Povolte moderní ověřování](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) pro klienta Office.

Další informace najdete v tématu [řešení potíží s neprohlížeči, které se nedají přihlásit k Microsoft 365, Azure nebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

