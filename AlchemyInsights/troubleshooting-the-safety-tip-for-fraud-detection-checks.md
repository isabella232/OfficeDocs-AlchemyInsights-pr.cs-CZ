---
title: Řešení potíží bezpečnostní tip pro kontroly zjišťování podvodů
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955959"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Řešení potíží bezpečnostní tip pro kontroly zjišťování podvodů

Pokud se vám zobrazí zpráva bezpečnostní tip která říká, že odesílatel neprošel našimi kontrolami zjišťování podvodů a nemusí být tím, kým se jeví, pak odesílatel neprošel kontrolami ověřování DKIM nebo SPF. Nejlepší způsob, jak to vyřešit, je, aby odesílatel autorizuje sám sebe. Pokud odesílatel posílá vaším jménem, musíte ho autorizovat přidáním IP adresy odesílatele do záznamu SPF.
  
Další informace najdete v tématu Řešení [bezpečnostní tip (podezřelých)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) informací o kontrolách zjišťování podvodů.
  
Tady jsou některé další odkazy, které vám pomůžou:
  
- [Jak Microsoft používá rozhraní SPF (Sender Policy Framework) k zabránění falšování falšování](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Nastavení SPF, aby se zabránilo falšování falšování](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
