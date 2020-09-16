---
title: V klientovi Teams dochází k chybám?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691100"
---
# <a name="teams-client-crashing"></a>V klientovi Teams dochází k chybám?

Pokud v klientovi Teams dochází k chybám, vyzkoušejte následující postup:

- Pokud používáte desktopovou aplikaci Teams, [zkontrolujte, jestli je tato aplikace kompletně aktualizovaná](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Zkontrolujte, že jsou dostupné všechny [adresy URL a rozsahy Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) .

- Přihlaste se pomocí účtu správce tenanta a ověřte [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) , že neexistuje výpadek nebo snížení služby.

- Odinstalace a přeinstalace aplikace Teams (odkaz)
    - Přejděte do složky%appdata%\Microsoft\teams\ na počítači a odstraňte všechny soubory v tomto adresáři.
    - [Stáhněte a nainstalujte aplikaci Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a pokud je to možné, nainstalujte týmy jako správce (klikněte pravým tlačítkem na instalační program teams a vyberte Spustit jako správce, pokud je dostupný).

Pokud se klientu Teams pořád zhroutí, můžete problém vyřešit? Pokud ano:

1. Postupujte podle pokynů k postupu.
    - Zavřete všechny nepotřebné nebo důvěrné aplikace.
    - Spusťte nástroj Záznam postupu a reprodukovat tento problém pomocí příslušného uživatelského účtu.
    - [Shromážděte protokoly týmů, které zachycují zaznamenané kroky Reprodukujte](https://docs.microsoft.com/microsoftteams/log-files). **Poznámka**: Zkontrolujte, že máte Zachyťte přihlašovací adresu ovlivněného uživatele.
    - Shromážděte informace o výpisu nebo o bloku chyb (Windows). Spusťte Windows PowerShell v počítači, kde dochází k chybě, a spusťte následující příkazy:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Připojte soubor k případu podpory.
