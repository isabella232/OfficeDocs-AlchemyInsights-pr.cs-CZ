---
title: Řešení OneDrive chyb
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
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921000"
---
# <a name="troubleshoot-onedrive-crashes"></a>Řešení OneDrive chyb

Pokud OneDrive opakovaně dojde k chybě, zkuste tento postup řešení potíží:

**Ujistěte se, že nejsou nastavené klíče registru:**

1. Pomocí Editoru registru přejděte na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Pokud je funkce DisableFileSyncNGSC k dispozici a je nastavená na hodnotu 1, otevřete klávesu a změňte hodnotu na 0.
3. Ruční spuštění OneDrive na obrazovce Start ![Stiskněte klávesu Windows.](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), zadejte OneDrive do vyhledávacího pole a potom klikněte na OneDrive desktopové aplikace.

**Obnovení OneDrive:**

Poznámky:

- Obnovením OneDrive odpojíte všechna existující synchronizační připojení (včetně osobních OneDrive, pokud je nastavené).
- Soubory ani data neztratíte resetováním OneDrive na počítači.

**Obnovení továrního nastavení OneDrive:**

1. Otevřete dialogové okno Spustit stisknutím klávesy Windows A.
2. Zadejte %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stiskněte OK. Může se krátce zobrazit příkazové okno.
3. Ruční spuštění OneDrive na obrazovce Start ![Stiskněte klávesu Windows.](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), zadejte OneDrive do vyhledávacího pole a potom klikněte na OneDrive desktopové aplikace.

Poznámky:

- Pokud jste se rozhodli synchronizovat jenom některé složky před obnovením továrního nastavení, budete to muset udělat znovu po dokončení synchronizace. Další [informace najdete v OneDrive, které složky](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)se mají synchronizovat s   počítačem.
- Tento proces budete muset dokončit pro osobní OneDrive a OneDrive pro firmy.