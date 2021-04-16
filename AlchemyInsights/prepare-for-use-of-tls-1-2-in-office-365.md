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
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="16147-102">Příprava na používání protokolu TLS 1.2 v Microsoftu 365</span><span class="sxs-lookup"><span data-stu-id="16147-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="16147-103">Od 31. října 2018 bude pokračovat přechod Microsoftu 365 na protokol TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="16147-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="16147-104">Od 15. října 2020 začne O365 vypisovat tls 1.0 a 1.1 v celé službě.</span><span class="sxs-lookup"><span data-stu-id="16147-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="16147-105">Zahájení této změny bude pokračovat v několika příštích týdnech a měsících, ale zákazníci by měli předpokládat, že žádné hovory TLS 1.0/1.1 nebudou fungovat při zapojení do O365 od 15. října 2020.</span><span class="sxs-lookup"><span data-stu-id="16147-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="16147-106">Jak jsme již dříve sdělili (MC126199 v prosinci 2017, MC128929 v únoru 2018, MC186827 v červenci 2019 a MC218794 v červenci 2020), přesouváme všechny naše online služby na TLS (Transport Layer Security) 1.2+, aby bylo zajištěno nejlepší šifrování ve třídě a aby byla naše služba ve výchozím nastavení bezpečnější.</span><span class="sxs-lookup"><span data-stu-id="16147-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="16147-107">Zákazníci si pořád mohou zvolit, jestli mají tls 1.0/1.1 na svých serverech a zdrojích, ale měli by předpokládat, že při interakci se zdroji O365 bude fungovat jenom TLS 1.2 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="16147-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="16147-108">Další informace o těchto změnách najdete [tady](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) [a tady.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="16147-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  