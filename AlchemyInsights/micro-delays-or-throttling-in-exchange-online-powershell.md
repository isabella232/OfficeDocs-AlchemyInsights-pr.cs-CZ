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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868527"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrozpoždění a omezování v Exchange Online PowerShellu

Když spustíte skripty a rutiny v Exchangi Online, mohou se zobrazit upozornění „Použito mikrozpoždění“ nebo se objevit zpoždění. Tady je několik návrhů, jak to vyřešit:

- Spusťte prosím naši diagnostiku, abyste uvolnili zásady omezení PowerShellu vašeho tenanta. Toto řešení vyřeší problém většinou.
- Pokud se problém stále nevyřeší, použijte [modul Exchange Online v2 PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), který zahrnuje cmdlety, které jsou založené na rozhraní REST API a jsou podstatně výkonnější. Může to být skvělé řešení pro velké množství často používaných rutin Get-.
- Pokud potřebujete používat cmdlety, které nejsou zahrnuté v modulu v2, přečtěte si prosím téma Spouštění rutin [PowerShellu](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)pro velký počet uživatelů v Office 365 , který hovoří o tom, jak obcházet limity omezení PowerShellu v Exchange Online.
