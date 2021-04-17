---
title: Poradce při potížích s chybou OneDrivu
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826192"
---
# <a name="troubleshoot-onedrive-crashes"></a>Poradce při potížích s chybou OneDrivu

Pokud onedrive opakovaně dochází k chybě, zkuste tento postup řešení potíží:

**Ujistěte se, že nejsou nastavené klíče registru:**

1. Pomocí Editoru registru přejděte na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Pokud je funkce DisableFileSyncNGSC k dispozici a je nastavená na hodnotu 1, otevřete klávesu a změňte hodnotu na 0.
3. Ruční spuštění OneDrivu tak, že půjdete na Start ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhledávacího pole zadejte OneDrive a klikněte na desktopové aplikaci OneDrive.

**Resetování OneDrivu:**

Poznámky:

- Resetováním OneDrivu se odpojí všechna stávající synchronizační připojení (včetně osobního OneDrivu při nastavení).
- Soubory ani data neztratíte resetováním OneDrivu na počítači.

**Resetování OneDrivu:**

1. Otevřete dialogové okno Spustit stisknutím klávesy Windows a klávesy R.
2. Zadejte %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stiskněte OK. Může se krátce zobrazit příkazové okno.
3. Ruční spuštění OneDrivu tak, že půjdete na Start ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhledávacího pole zadejte OneDrive a klikněte na desktopové aplikaci OneDrive.

Poznámky:

- Pokud jste se rozhodli synchronizovat jenom některé složky před obnovením továrního nastavení, budete to muset udělat znovu po dokončení synchronizace. Přečtěte [si informace o tom, které složky OneDrivu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)se mají synchronizovat s   počítačem.
- Tento proces budete muset dokončit pro svůj osobní OneDrive a OneDrive pro firmy.