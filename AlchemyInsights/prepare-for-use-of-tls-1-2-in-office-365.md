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
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040391"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Příprava na používání protokolu TLS 1.2 v Microsoftu 365

Od 31. října 2018 bude pokračovat přechod Microsoftu 365 na protokol TLS 1.2. Od 15. října 2020 začne O365 vypisovat tls 1.0 a 1.1 v celé službě. Zahájení této změny bude pokračovat v několika příštích týdnech a měsících, ale zákazníci by měli předpokládat, že žádné hovory TLS 1.0/1.1 nebudou fungovat při zapojení do O365 od 15. října 2020. Jak jsme již dříve sdělili (MC126199 v prosinci 2017, MC128929 v únoru 2018, MC186827 v červenci 2019 a MC218794 v červenci 2020), přesouváme všechny naše online služby na TLS (Transport Layer Security) 1.2+, aby bylo zajištěno nejlepší šifrování ve třídě a aby byla naše služba ve výchozím nastavení bezpečnější. Zákazníci si pořád mohou zvolit, jestli mají tls 1.0/1.1 na svých serverech a zdrojích, ale měli by předpokládat, že při interakci se zdroji O365 bude fungovat jenom TLS 1.2 nebo novější.
  
Další informace o těchto změnách najdete [tady](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [a tady.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)

  