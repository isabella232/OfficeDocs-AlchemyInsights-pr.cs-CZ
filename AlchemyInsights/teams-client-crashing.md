---
title: Teams klienta dojde k chybě
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187714"
---
# <a name="teams-client-crashing"></a>Teams klienta dojde k chybě

Pokud v klientovi Teams dochází k chybám, vyzkoušejte následující postup:

- Pokud používáte desktopovou aplikaci Teams, [zkontrolujte, jestli je tato aplikace kompletně aktualizovaná](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Ujistěte se, [že jsou Microsoft 365 adresy URL a rozsahy adres](/microsoftteams/connectivity-issues) přístupné.

- Přihlaste se pomocí účtu správce tenanta a zkontrolujte řídicí panel [stavu služby,](/office365/enterprise/view-service-health) abyste ověřili, že neexistuje žádný výpadk nebo degradace služby.

- Odinstalace a přeinstalace Teams aplikace
    - Přejděte do složky %appdata%\Microsoft\Teams\ na počítači a odstraňte všechny soubory v tomto adresáři.
    - [Stáhněte a nainstalujte aplikaci Teams a](https://www.microsoft.com/microsoft-teams/download-app)pokud je to možné, nainstalujte Teams jako správce (klikněte  pravým tlačítkem na instalační program Teams a vyberte Spustit jako správce, pokud je k dispozici).

Pokud váš Teams klient stále dochází k chybě, zkuste problém reprodukovat. Pokud můžete:

1. K zachycení kroků použijte Záznam kroků.
    - Zavřete všechny nepotřebné nebo důvěrné aplikace.
    - Spusťte záznam kroků a reprodukovat problém při přihlášení pomocí ovlivněného uživatelského účtu.
    - [Shromážděte protokoly týmů, které zaznamenávají zaznamenané kroky reprocesu](/microsoftteams/log-files). **Poznámka:** Ujistěte se, že zaznamenáte přihlašovací adresu ovlivněné uživatele.
    - Shromážděte informace o kontejneru stavu a/nebo chybovém kontejneru (Windows). Spusťte Windows powershellu na počítači, kde k chybě dochází, a spusťte následující příkazy (po každém příkazu stiskněte Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Po vygenerování textového souboru, který se zobrazí na obrazovce, uložte soubor a připojte ho k žádosti o službu. 
