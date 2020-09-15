---
title: Řešení potíží s bezpečnostním tipem pro kontroly rozpoznávání podvodů
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658403"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Řešení potíží s bezpečnostním tipem pro kontroly rozpoznávání podvodů

Pokud se vám zobrazuje bezpečnostní tip, který říká "odesílatel selhal při kontrole vyhledávání podvodů a nepovažuje se, kdo se jeví jako", odesílatel se nepovedlo projít kontrolou ověřování DKIM nebo SPF. Nejlepším způsobem, jak tento problém vyřešit, je to, aby ho odesílatel sám povolil. Pokud odesílatel posílá vaše zastoupení, musíte ho schválit přidáním IP adresy odesílatele k záznamu SPF.
  
Další informace najdete v článku [Poradce při potížích s červeným (podezřelým) bezpečnostním tipem pro detekci podvodů](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Tady je několik dalších odkazů, které vám můžou pomoct:
  
- [Jak Microsoft používá k zabránění falšování identity architekturu zásad pro odesílatele (SPF)](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Nastavení SPF pro zabránění falšování obsahu](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
