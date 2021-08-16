---
title: Jak zakázat externí skupiny
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015613"
---
# <a name="how-to-disable-external-groups"></a>Jak zakázat externí skupiny

Yammer externí zasílání zpráv se Exchange transportních pravidel (ETR), sady proaktivních ovládacích prvků, které brání sdílení informací o společnosti. Pokud chcete uživatelům omezit vytváření externích skupin, musíte nakonfigurovat pravidlo přenosu Exchange (ETR) Exchange potom nakonfigurovat Yammer tak, aby k blokování externích zpráv Exchange použít pravidlo přenosu Exchange.
  
Po vytvoření pravidla v Centru Exchange Online pro správu nastavte etr tak, aby se v Yammer:
  
- Přihlaste se k Yammer jako ověřený správce a v Centru pro správu **Yammer** přejděte na C **Content and Security Security \> Nastavení.**

- V **části Externí zasílání** zpráv vyberte vynutit Exchange Online Exchange pravidel přenosu **(ETR) v Yammer.**

- Zvolte **Uložit**.

Další informace najdete v tématu [Zakázání externích zpráv](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)v Yammer síti .
  