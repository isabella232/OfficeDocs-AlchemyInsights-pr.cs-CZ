---
title: Pracovní postup se nezahajuje.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403736"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="82750-102">Pracovní postup se nezahajuje.</span><span class="sxs-lookup"><span data-stu-id="82750-102">Workflow is not starting</span></span>

- <span data-ttu-id="82750-103">Pracovní postupy SharePointu 2010 a SharePointu 2013 se nezahajuje.</span><span class="sxs-lookup"><span data-stu-id="82750-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="82750-104">Pokud pracovní postup nezačáte, může docházet k dočasnému problému se službou, kdy se uživatelům může při průběhu pracovního postupu občas vyskytnout zpoždění.</span><span class="sxs-lookup"><span data-stu-id="82750-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="82750-105">Zkontrolujte řídicí [panel Stavu služby](https://admin.microsoft.com/AdminPortal/Home/servicehealth) a podívejte se, jestli má vaše organizace vliv.</span><span class="sxs-lookup"><span data-stu-id="82750-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="82750-106">Pokud od prvního pohledu na tento problém uplynulo více než 24 hodin, přihlaste se prosím k lístku podpory.</span><span class="sxs-lookup"><span data-stu-id="82750-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="82750-107">V mnoha případech už pracujeme na řešení.</span><span class="sxs-lookup"><span data-stu-id="82750-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="82750-108">Na dokončení řešení nám prosím dejte aspoň 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="82750-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="82750-109">Pracovní postupy SharePointu 2010 se zpozdí při spuštění.</span><span class="sxs-lookup"><span data-stu-id="82750-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="82750-110">K tomu dochází, pokud se pracovní postup aktivuje ve velkých dávkách.</span><span class="sxs-lookup"><span data-stu-id="82750-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="82750-111">(například když se přidá několik položek najednou).</span><span class="sxs-lookup"><span data-stu-id="82750-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="82750-112">Pracovní postupy nejsou navržené tak, aby spouštěly v reálném čase, takže zpoždění je chování podle návrhu.</span><span class="sxs-lookup"><span data-stu-id="82750-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="82750-113">Pokud je pracovní postup složitý, může být kompilace pomalá.</span><span class="sxs-lookup"><span data-stu-id="82750-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="82750-114">Podívejte [se na tento](https://support.microsoft.com//kb/3043697) článek.</span><span class="sxs-lookup"><span data-stu-id="82750-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="82750-115">Pracovní postup byste měli zjednodušit nebo ho předělat pomocí typu platformy Microsoft SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="82750-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="82750-116">Pokud se historie pracovních postupů rozrostla, možná budete chtít položky vymazat nebo vytvořit nový seznam historie.</span><span class="sxs-lookup"><span data-stu-id="82750-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="82750-117">Další informace: [Vymazání historie pracovních postupů](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="82750-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="82750-118">Související témata</span><span class="sxs-lookup"><span data-stu-id="82750-118">Related topics</span></span>
<span data-ttu-id="82750-119">Chcete vyzkoušet Microsoft Flow v SharePointu Online?</span><span class="sxs-lookup"><span data-stu-id="82750-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="82750-120">Vytvoření toku</span><span class="sxs-lookup"><span data-stu-id="82750-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="82750-121">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="82750-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
