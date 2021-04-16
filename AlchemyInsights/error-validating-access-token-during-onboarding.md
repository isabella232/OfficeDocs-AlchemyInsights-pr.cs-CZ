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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813681"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Chyba při ověřování přístupového tokenu při desktopové analýze

Tato chyba se obvykle pozoruje, když vyprší platnost ověřovacího tokenu. Aktualizace stránky obvykle aktualizuje token. Tento problém ale může přetrvávat, pokud existují nějaké zásady podmíněného přístupu použité u účtu používaného k místní desktopové analýze. Na portálu Azure Portal si můžete zkontrolovat protokoly přihlášení k Azure AD a zjistit, jestli u účtu používaného pro přihlášení k desktopové analýze došlo k chybě přihlášení.

Další informace o podmíněném přístupu najdete na webu [Plánování nasazení podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).