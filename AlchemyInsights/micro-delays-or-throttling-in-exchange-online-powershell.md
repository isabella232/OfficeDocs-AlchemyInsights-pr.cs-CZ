---
title: Mikrozpoždění a omezování v Exchange Online PowerShellu
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702119"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrozpoždění a omezování v Exchange Online PowerShellu

Když spustíte skripty a rutiny v Exchangi Online, mohou se zobrazit upozornění „Použito mikrozpoždění“ nebo se objevit zpoždění. Tady je několik návrhů, jak to vyřešit:

- Spusťte prosím naši diagnostiku, abyste uvolnili zásady omezení PowerShellu vašeho tenanta. Toto řešení vyřeší problém většinou.
- Pokud se problém stále nevyřeší, použijte [modul PowerShellu Exchange Online verze 2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)který zahrnuje cmdlety, které jsou založené na rozhraní REST API a jsou podstatně výkonnější. Může to být skvělé řešení pro velké množství často používaných rutin Get-.
- Pokud potřebujete používat cmdlety, které nejsou zahrnuté v modulu v2, přečtěte si prosím téma Spouštění rutin [PowerShellu](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)pro velký počet uživatelů v Office 365 , který hovoří o tom, jak se v Exchange Online obekat omezení PowerShellu.
