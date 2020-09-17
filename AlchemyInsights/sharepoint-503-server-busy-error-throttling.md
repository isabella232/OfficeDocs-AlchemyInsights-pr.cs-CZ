---
title: Omezování SharePointu Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773840"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="94700-102">Omezování SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="94700-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="94700-103">**Důležité**: V této mimořádné době přijímáme opatření, aby služby SharePointu Online a OneDrivu zůstaly vysoce dostupné. Další informace najdete v článku zaměřeném na [dočasné úpravy funkcí SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="94700-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="94700-104">**503 Server je zaneprázdněný**</span><span class="sxs-lookup"><span data-stu-id="94700-104">**503 server is busy error**</span></span>

<span data-ttu-id="94700-105">Při pokusu o přechod na weby SharePointu nebo OneDrivu může dojít k chybě serveru 503.</span><span class="sxs-lookup"><span data-stu-id="94700-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="94700-106">Tato chyba může být způsobena omezením služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="94700-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="94700-107">SharePoint Online využívá omezování k zajištění optimálního výkonu a spolehlivosti svých služeb.</span><span class="sxs-lookup"><span data-stu-id="94700-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="94700-108">Omezování limituje počet akcí uživatelů nebo současných volání (podle skriptů nebo kódu), aby nedocházelo k nadměrnému využití prostředků.</span><span class="sxs-lookup"><span data-stu-id="94700-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="94700-109">Další informace o omezování najdete [v článku Neomezovat nebo zablokovat v SharePointu Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="94700-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="94700-110">Pokud se domníváte, že tato chyba nesouvisí s omezením, můžete zkontrolovat, jestli se na vašem tenantovi nachází aktivní údržba, a to tak, že přejdete do [centra zpráv](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="94700-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="94700-111">Nakonec se ujistěte, že jste na stránce [stavu služby](https://portal.office.com/adminportal/home#/servicehealth) zkontrolovali všechny informační a incidenty, které se můžou vyskytovat.</span><span class="sxs-lookup"><span data-stu-id="94700-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

