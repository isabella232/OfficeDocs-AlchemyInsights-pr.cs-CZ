---
title: Oprava aplikací Microsoft 365
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747688"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Oprava aplikací Microsoft 365 se zprávou nenašly se licence Office přidružené.

Pokud se zobrazí tato zpráva, zkuste toto:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že nejsou blokovány internetové připojení k aplikacím Microsoft 365. Viz [adresy URL a rozsahy IP adres pro Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Odeberte a [přiřaďte licenci Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) příslušnému uživateli. 
3. Otevřete aplikaci Office a [odhlaste](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se z existujících uživatelských účtů.
4. Přejděte na nastavení Windows > **účty**  >  **e-mailem &** a odeberte všechny pracovní účty kromě příslušného účtu.
5. Přejděte na nastavení Windows > **účty**  >  **k práci nebo škole**a odpojte všechny pracovní účty kromě příslušného účtu.
6. Resetujte stav aktivace Office. [Zjistěte, jak](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Přihlaste](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) se pomocí příslušného uživatelského účtu.

Další řešení pro řešení potíží najdete [v článku chyby typu nelicencovaný produkt a chyby aktivace v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).