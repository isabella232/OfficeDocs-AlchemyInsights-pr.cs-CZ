---
title: Při nástupu do desktopové analýzy došlo k chybě při ověřování přístupového tokenu.
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
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946608"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Chyba při ověřování přístupového tokenu při desktopové analýze

Tato chyba se obvykle pozoruje, když vyprší platnost ověřovacího tokenu. Aktualizace stránky obvykle aktualizuje token. Tento problém ale může přetrvávat, pokud existují nějaké zásady podmíněného přístupu použité u účtu používaného k místní desktopové analýze. Na portálu Azure Portal si můžete zkontrolovat protokoly přihlášení k Azure AD a zjistit, jestli u účtu používaného pro přihlášení k desktopové analýze došlo k chybě přihlášení.

Další informace o podmíněném přístupu najdete na webu [Plánování nasazení podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).