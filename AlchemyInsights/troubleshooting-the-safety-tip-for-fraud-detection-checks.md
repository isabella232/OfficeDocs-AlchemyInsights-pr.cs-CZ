---
title: Řešení potíží s bezpečnostním tipem pro kontroly zjišťování podvodů
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834724"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Řešení potíží s bezpečnostním tipem pro kontroly zjišťování podvodů

Pokud se vám zobrazí bezpečnostní tip s informací, že odesílatel neprošel našimi kontrolami zjišťování podvodů a nemusí být tím, kým se jeví, pak odesílatel neprošel kontrolami ověřování DKIM nebo SPF. Nejlepší způsob, jak to vyřešit, je, aby odesílatel autorizuje sám sebe. Pokud odesílatel posílá vaším jménem, musíte ho autorizovat přidáním IP adresy odesílatele do záznamu SPF.
  
Další informace najdete v článku Řešení potíží s [červeným (podezřelým)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) bezpečnostním tipem pro zjišťování podvodů.
  
Tady jsou některé další odkazy, které vám pomůžou:
  
- [Jak Microsoft používá rozhraní SPF (Sender Policy Framework) k zabránění falšování falšování](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Nastavení SPF, aby se zabránilo falšování falšování](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
