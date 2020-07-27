---
title: Jednomu uživateli se při přidávání doplňků v Outlooku zobrazí chyba odepření přístupu.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 1f4672e306a282b3e1d20c75f4e361c02cdddaed
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423484"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Jednomu uživateli se při přidávání doplňků v Outlooku zobrazí chyba odepření přístupu.

Prostředí PowerShell uživatele Chcete-li najít oprávnění:

Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegování $false | Formát-Tabulka -Automatická role,Název_role,Typ přiřazení_role