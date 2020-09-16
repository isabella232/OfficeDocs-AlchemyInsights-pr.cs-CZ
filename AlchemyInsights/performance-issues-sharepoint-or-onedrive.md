---
title: Problémy s výkonem – SharePoint nebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771894"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="7c643-102">SharePoint nebo OneDrive pomalý, nedostupný ani nedostupný pro víc uživatelů</span><span class="sxs-lookup"><span data-stu-id="7c643-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="7c643-103">SharePoint nebo OneDrive můžou být pomalé, nepřístupné nebo nedostupné nebo nemusí být zobrazovat 503 služby, a to z několika důvodů:</span><span class="sxs-lookup"><span data-stu-id="7c643-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="7c643-104">Pokud je váš web SharePointu nebo OneDrivu pomalý nebo opožděný pro víc uživatelů, může se jednat o dočasný problém s tím, že uživatelé při přístupu k SharePointovým webům nebo obsahu OneDrivu zastupují.</span><span class="sxs-lookup"><span data-stu-id="7c643-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="7c643-105">Podívejte se na [řídicí panel stavu služeb](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) a zjistěte, jestli je vaše organizace ovlivněná.</span><span class="sxs-lookup"><span data-stu-id="7c643-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="7c643-106">Při pokusu o přechod na weby SharePointu nebo OneDrivu může dojít k chybě *serveru 503* .</span><span class="sxs-lookup"><span data-stu-id="7c643-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="7c643-107">Tato chyba může být způsobena omezením služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7c643-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="7c643-108">SharePoint Online využívá omezování k zajištění optimálního výkonu a spolehlivosti svých služeb.</span><span class="sxs-lookup"><span data-stu-id="7c643-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="7c643-109">Omezování limituje počet akcí uživatelů nebo současných volání (podle skriptů nebo kódu), aby nedocházelo k nadměrnému využití prostředků.</span><span class="sxs-lookup"><span data-stu-id="7c643-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="7c643-110">Další informace o omezování najdete [v článku Neomezovat nebo zablokovat v SharePointu Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="7c643-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="7c643-111">Pokud se setkáte s nízkým výkonem při používání **klasického** nebo **moderního** webu nebo stránky SharePointu, analyzujte stránky pomocí [nástroje Diagnostika stránky](https://aka.ms/perftool) .</span><span class="sxs-lookup"><span data-stu-id="7c643-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="7c643-112">Pokud pořád dochází k obecnému snížení výkonu, podívejte se na materiály v dolní části tohoto článku: [Úvod k ladění výkonu pro SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="7c643-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  