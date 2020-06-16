---
title: Poradce při potížích s havárií OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748795"
---
# <a name="troubleshoot-onedrive-crashes"></a>Poradce při potížích s havárií OneDrivu

Pokud OneDrive opakovaně havaruje, vyzkoušejte tyto kroky pro řešení potíží:

**Ujistěte se, že klíče registru nejsou nastaveny:**

1. Pomocí Editoru registru přejděte na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Pokud disableFileSyncNGSC je k dispozici a nastavte na hodnotu 1, otevřete klíč a změňte hodnotu na 0.
3. Ruční spuštění OneDrivu tak, že přejdete na úvodní obrazovku ![Stisknutí klávesy Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), zadejte do vyhledávacího pole OneDrive a klikněte na desktopovou aplikaci OneDrive.

**Resetování OneDrivu:**

Poznámky:

- Resetováním OneDrivu odpojíte všechna stávající synchronizační připojení (včetně osobního OneDrivu, pokud je nastavený).
- O soubory ani data nedojde resetováním OneDrivu v počítači.

**Resetování OneDrivu:**

1. Otevřete dialogové okno Spustit stisknutím klávesy Windows a R.
2. Zadejte %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stiskněte OK. Krátce se může zobrazit okno příkazu.
3. Ruční spuštění OneDrivu tak, že přejdete na úvodní obrazovku ![Stisknutí klávesy Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), zadejte do vyhledávacího pole OneDrive a klikněte na desktopovou aplikaci OneDrive.

Poznámky:

- Pokud jste se rozhodli synchronizovat pouze některé složky před resetováním, budete to muset udělat znovu po dokončení synchronizace. Další informace [načtěte: Zvolte, které složky OneDrivu se mají synchronizovat s](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   počítačem.
- Budete to muset dokončit pro osobní OneDrive a OneDrive pro firmy.