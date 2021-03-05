---
title: O Exchange Server aktualizací zabezpečení
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481120"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="aeb45-102">O Exchange Server aktualizací zabezpečení</span><span class="sxs-lookup"><span data-stu-id="aeb45-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="aeb45-103">Microsoft vydal řadu důležitých aktualizací zabezpečení pro Exchange Server místního nasazení.</span><span class="sxs-lookup"><span data-stu-id="aeb45-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="aeb45-104">Ovlivněné verze serveru jsou všechny úrovně aktualizací Exchange Server 2010, 2013, 2016 a 2019.</span><span class="sxs-lookup"><span data-stu-id="aeb45-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="aeb45-105">Exchange Online není ovlivněný, ale pokud máte některé místní servery Exchange kvůli hybridní konfiguraci, potenciálně mohou být ohrožené.</span><span class="sxs-lookup"><span data-stu-id="aeb45-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="aeb45-106">Abyste mohli aktualizovat místní servery, musí běžet aspoň na těchto verzích Exchange:</span><span class="sxs-lookup"><span data-stu-id="aeb45-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="aeb45-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="aeb45-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="aeb45-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="aeb45-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="aeb45-109">Exchange Server 2016 CU 19 nebo CU 18</span><span class="sxs-lookup"><span data-stu-id="aeb45-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="aeb45-110">Exchange Server 2019 CU 8 nebo CU 7</span><span class="sxs-lookup"><span data-stu-id="aeb45-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="aeb45-111">Podívejte se prosím na následující oznámení o umístění oprav: Vydaná: Aktualizace zabezpečení z března [2021 Exchange Server 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="aeb45-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="aeb45-112">**Důležité poznámky:**</span><span class="sxs-lookup"><span data-stu-id="aeb45-112">**Important notes:**</span></span>

<span data-ttu-id="aeb45-113">Instalace aktualizací nebude fungovat, pokud na vašich místních serverech nejsou spuštěné požadované verze Exchange podle výše uvedeného seznamu.</span><span class="sxs-lookup"><span data-stu-id="aeb45-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="aeb45-114">Pokud aktualizace instalujete ručně, přečtěte si důležité informace v článku znalostní báze o známých problémech.</span><span class="sxs-lookup"><span data-stu-id="aeb45-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="aeb45-115">Ze zvýšených pokynů CMD/PowerShellu musí být spuštěny aktualizace zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="aeb45-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
