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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709099"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is notfunctioning properly" message

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Nainstalujte nejnovější aktualizace [pro Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) pomocí Správce přihlašovacích údajů systému Windows.<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Zkuste [chyby MODULU](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) DŮVĚRYHODNÉ PLATFORMY (MODULEM) opravit procesem obnovení uživatele.
- Nastavte enableADAL = 0 pomocí následujících kroků:  
    1. Klikněte pravým tlačítkem myši na tlačítko Start systému Windows, zvolte **Spustit,** zadejte **regedit** a pak zvolte **OK.**
    2. Výběrem **možnosti** Ano povolíte Editoru registru dělat změny na vašem zařízení.
    3. V Editoru registru přidejte hodnotu DWORD **EnableADAL** s nastavením **0** v HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Další informace najdete v článku Problémy s připojením při přihlašování po aktualizaci na [build Office 2016 16.0.7967 ve Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)