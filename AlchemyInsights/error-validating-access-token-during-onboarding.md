---
title: Došlo k chybě při ověřování tokenu přístupu v průběhu analýzy na ploše.
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783544"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Při prověřování desktopové analýzy došlo k chybě při ověřování tokenu přístupu

Tato chyba se obvykle zobrazuje, když vyprší platnost ověřovacího tokenu. Obvykle se aktualizace stránky aktualizuje. Tento problém ale může trvat i v případě, že jsou u účtu, který se používá k analýze desktopové analýzy, všechny zásady podmíněného přístupu. V protokolech Azure AD se můžete podívat do protokolů v Azure Portalu a zjistit, jestli nedochází k chybám přihlašování pro účet, který se používá pro službu Desktop Analytics.

Další informace o podmíněném přístupu najdete v tématu [Plánování nasazení podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).