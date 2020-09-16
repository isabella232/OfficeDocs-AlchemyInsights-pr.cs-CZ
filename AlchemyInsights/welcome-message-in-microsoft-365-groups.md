---
title: Uvítací zpráva ve skupinách Microsoft 365
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
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725832"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Uvítací zpráva ve skupinách Microsoft 365

Noví uživatelé, kteří se připojují ke skupině Microsoft 365, obdrží uvítací e-mail, pokud má vlastnost "UnifiedGroupWelcomeMessageEnabled" hodnotu true.

Pokud chcete uvítací zprávu zakázat, použijte následující [EXO příkaz PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) :

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
