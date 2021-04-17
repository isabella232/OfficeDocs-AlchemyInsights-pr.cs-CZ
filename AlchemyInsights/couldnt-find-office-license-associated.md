---
title: 'Oprava aplikací Microsoft 365: Nenašli jsme přidruženou zprávu o licencích office.'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816481"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Oprava zprávy o tom, že aplikace Microsoft 365 nejsou přidružené k licencím office

Pokud se vám tato zpráva zobrazí, zkuste toto:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že neblokují přístup k internetu k aplikacím Microsoft 365. Viz Adresy URL a rozsahy IP adres [microsoftu 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Odeberte [a znovu přijměte licenci Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pro postiženého uživatele. 
3. Otevřete aplikaci Office a [odhlásit se od](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) všech existujících uživatelských účtů.
4. Přejděte na Nastavení Windows > **Účty**  >  **e-& účty** a odeberte všechny pracovní účty kromě ovlivněného účtu.
5. Přejděte na Nastavení Systému Windows > **účty Access** v práci nebo ve škole a odpojte všechny pracovní účty kromě  >  ovlivněného účtu.
6. Resetujte stav aktivace Office. [Zjistěte, jak](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)na to.
7. [Přihlaste se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.

Další řešení pro řešení potíží najdete v [článku Chyby nelicencovaných](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)produktů a aktivace v Office .