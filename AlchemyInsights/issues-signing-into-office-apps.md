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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986884"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Oprava Microsoft 365 aplikace "Modul důvěryhodné platformy vašeho počítače nefunguje správně".

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Nainstalujte si nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [a Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Vymažte Office přihlašovací údaje](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Správce přihlašovacích údajů.<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Zkuste [proces obnovení uživatele a](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opravte chyby modulu ČIPM (Trusted Platform Module).
- Pomocí následujících kroků nastavte EnableADAL = 0:  
    1. Klikněte pravým tlačítkem myši na Windows Start, zvolte **Spustit,** zadejte **regedit** a pak zvolte **OK.**
    2. Výběrem **možnosti Ano** povolíte Editoru registru provádět změny ve vašem zařízení.
    3. V Editoru registru přidejte hodnotu DWORD **EnableADAL** s nastavením **0** v části HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Další informace najdete v článku Problémy s připojením při přihlašování po aktualizaci na [Office 2016 build 16.0.7967 v Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).