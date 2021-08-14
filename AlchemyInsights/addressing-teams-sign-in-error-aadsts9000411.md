---
title: Addressing Teams sign-in error AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953008"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Addressing Teams sign-in error AADSTS9000411

Při přihlašování k Microsoft Teams se může zobrazit chybová zpráva: Omlouváme se, ale máme potíže s přihlášením v **aplikaci AADSTS9000411: Žádost není správně naformátovaná. Parametr "login_hint" se duplikuje.**

Pokud chcete tento problém vyřešit, ujistěte se, Microsoft Teams se aktualizují vaši klienti. Další informace o aktualizaci klienta najdete v tématu [Aktualizace Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Pokud klienta z nějakého důvodu nemůžete aktualizovat, odhlášení klienta vymaže většinu dat uložených v mezipaměti. Pokud ale po odhlášení nebo přihlášení pořád máte problémy, ukončete Teams a vymažte mezipaměť klienta takto:
1. Zavřete Microsoft Teams.
2. Přejděte na: %appdata%\microsoft\teams a odstraňte všechny soubory.
3. Znovu otevřete Microsoft Teams.
