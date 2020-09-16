---
title: Chyba při přihlašování týmů pro adresování AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687031"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Chyba při přihlašování týmů pro adresování AADSTS9000411

Při přihlášení k Microsoft Teams se může zobrazit chyba: Bohužel máme **problémy s přihlášením v AADSTS9000411: žádost nemá správný formát. Parametr "login_hint" je duplicitní.**

Pokud chcete tento problém vyřešit, zkontrolujte, jestli máte aktualizované klienty Microsoft Teams. Další informace o aktualizaci klienta najdete v článku [aktualizace Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Pokud z nějakého důvodu nemůžete klienta aktualizovat, odhlášení klienta vymaže data z mezipaměti. Pokud ale máte problémy i po odhlášení nebo přihlášení, zavřete aplikace teams a zrušte zaškrtnutí následujícího:
1. Ukončete aplikaci Microsoft Teams.
2. Přejděte na:%AppData%\microsoft\teams a odstraňte všechny soubory.
3. Znovu spusťte aplikaci Microsoft Teams.
