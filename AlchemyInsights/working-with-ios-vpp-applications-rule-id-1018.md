---
title: Práce s aplikacemi VPP v systému iOS – ID pravidla 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688939"
---
# <a name="working-with-ios-vpp-applications"></a>Práce s aplikacemi VPP v iOS

Přečtěte si, [jak spravovat aplikace pro iOS zakoupené prostřednictvím programu Volume-purchase s Microsoft Intune s](https://docs.microsoft.com/intune/vpp-apps-ios) informacemi o funkcích, omezeních a krocích, jak používat program Apple Volume purchase a podporu pro něj v Microsoft Intune.
  
 **Běžné problémy:** "Přidělil (a) aplikaci VPP aplikace Skype, ale instalace se nezdařila."
  
- K tomu může dojít, pokud je jeden token VPP použit napříč více poskytovateli správy mobilních zařízení. Tokeny VPP z Apple se můžou používat jenom s jedním poskytovatelem. Pokud jste použili token VPP s víc poskytovateli, musíte ho znovu nahrát do Intune.

- Instalace se může zdařit také v případě, že celkový počet instalací přesáhne počet licencí. Pokud chcete zobrazit sestavu využití licencí, přejděte na stránku aplikace **Intune Mobile Apps** – \> **licence** . Informace o tom, jak si vyžádat licence používané, najdete v [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
