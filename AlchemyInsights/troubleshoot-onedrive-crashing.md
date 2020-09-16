---
title: Odstraňování potíží s OneDrivem
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664991"
---
# <a name="troubleshoot-onedrive-crashes"></a>Odstraňování potíží s OneDrivem

Pokud se OneDrive opakovaně zhroutí, zkuste tyto kroky:

**Zkontrolujte, jestli nejsou nastavené klíče registru:**

1. Použití Editoru registru, přejděte na HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Pokud je DisableFileSyncNGSC přítomen a je nastaven na 1, otevřete klíč a změňte hodnotu na 0.
3. Ruční spuštění OneDrivu tak, že přejdete na Start ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhledávacího pole zadejte OneDrive a klikněte na desktopovou aplikaci OneDrive.

**Resetování OneDrivu:**

Komentář

- Obnovením OneDrivu se odpojí všechna vaše stávající synchronizovaná připojení (včetně osobního OneDrivu, pokud je nastavená).
- Obnovením OneDrivu na počítači nepřijdete o soubory ani data.

**Obnovení OneDrivu:**

1. Stisknutím kláves Windows a R otevřete dialogové okno spustit.
2. Zadejte% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset a stiskněte OK. Krátce se zobrazí okno příkazového řádku.
3. Ruční spuštění OneDrivu tak, že přejdete na Start ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhledávacího pole zadejte OneDrive a klikněte na desktopovou aplikaci OneDrive.

Komentář

- Pokud jste se rozhodli synchronizovat jenom některé složky před obnovením, budete se muset pokusit po dokončení synchronizace. Přečtěte si o [tom, které složky OneDrivu se mají synchronizovat s počítačem](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85),   kde najdete další informace.
- Tento postup musíte provést pro svůj osobní OneDrive a OneDrive pro firmy.