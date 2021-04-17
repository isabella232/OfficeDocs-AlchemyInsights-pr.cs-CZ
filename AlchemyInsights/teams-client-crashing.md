---
title: V klientovi Teams dochází k chybám?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826264"
---
# <a name="teams-client-crashing"></a>V klientovi Teams dochází k chybám?

Pokud v klientovi Teams dochází k chybám, vyzkoušejte následující postup:

- Pokud používáte desktopovou aplikaci Teams, [zkontrolujte, jestli je tato aplikace kompletně aktualizovaná](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Ujistěte se, že jsou dostupné všechny adresy URL a rozsahy adres microsoftu [365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Přihlaste se pomocí účtu správce tenanta a zkontrolujte řídicí panel [stavu služby,](https://docs.microsoft.com/office365/enterprise/view-service-health) abyste ověřili, že neexistuje žádný výpadk nebo degradace služby.

- Odinstalace a přeinstalace aplikace Teams (odkaz)
    - Přejděte do složky %appdata%\Microsoft\teams\ na počítači a odstraňte všechny soubory v tomto adresáři.
    - [Stáhněte a nainstalujte aplikaci Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a pokud je to možné, nainstalujte Teams jako správce (klikněte pravým tlačítkem na instalační program Teams a vyberte "Spustit jako správce", pokud je k dispozici).

Pokud váš klient Teams pořád dochází k chybě, můžete problém reprodukovat? Pokud ano:

1. K zachycení kroků použijte Záznam kroků.
    - Zavřete všechny nepotřebné nebo důvěrné aplikace.
    - Spusťte záznam kroků a reprodukovat problém při přihlášení pomocí ovlivněného uživatelského účtu.
    - [Shromážděte protokoly týmů, které zaznamenávají zaznamenané kroky reprocesu](https://docs.microsoft.com/microsoftteams/log-files). **Poznámka:** Ujistěte se, že zaznamenáte přihlašovací adresu ovlivněné uživatele.
    - Shromážděte informace o kontejneru stavu a/nebo chybovém kontejneru (Windows). Spusťte Windows PowerShell na počítači, kde k chybě dochází, a spusťte následující příkazy:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Připojte soubor k případu podpory.
