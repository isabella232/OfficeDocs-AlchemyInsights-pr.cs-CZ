---
title: Příprava na používání protokolu TLS 1.2 v Microsoftu 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085897"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Příprava na používání protokolu TLS 1.2 v Microsoftu 365

Od 31. října 2018 bude pokračovat přechod Microsoftu 365 na protokol TLS 1.2. Od 2020 15. října 365 zahájí neplatnost protokolu TLS 1,0 a 1,1 v této službě. Zavedení této změny bude pokračovat během příštích několika týdnů a měsíců, ale zákazníci by neměli předpokládat, že budou mít hovory TLS 1.0/1.1 fungovat při práci se službou O365 ve spuštění 15, 2020. Jak již dříve komunikoval (MC126199 v dec 2017, MC128929 v únoru 2018, MC186827 v červenci 2019, a MC218794 v červenci 2020), přenášíme všechny naše online služby na zabezpečení TLS (Transport Layer Security) 1.2 +, kde je k dispozici šifrování Best-in-class a že naše služby jsou ve výchozím nastavení bezpečnější. Zákazníci si přesto můžou na svých serverech a prostředích používat protokol TLS 1.0/1.1, ale měly by při práci s prostředky O365 začínat pouze TLS 1,2 nebo vyšší.
  
Další informace o těchto změnách najdete [tady](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) a [tady](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  