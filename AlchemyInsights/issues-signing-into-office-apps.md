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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695172"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Oprava aplikací Microsoft 365 "důvěryhodný čip TPM vašeho počítače nefunguje správně" zpráva

Pokud chcete tuto chybu vyřešit, vyzkoušejte následující:

- Nainstalujte si nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0. (Např.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Zkuste [obnovit](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) chyby čipu TPM (Trusted Platform Module).
- Nastavte EnableADAL = 0 pomocí následujících kroků:  
    1. Klikněte pravým tlačítkem myši na tlačítko Start systému Windows, zvolte **Spustit**, zadejte **Regedit**a pak zvolte **OK**.
    2. Výběrem možnosti **Ano** povolíte, aby Editor registru prováděl v zařízení změny.
    3. V editoru registru přidejte hodnotu DWORD pro **EnableADAL** s nastavením **0** v části HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Další informace najdete v článku [problémy s připojením při přihlášení po aktualizaci na Office 2016 Build 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).