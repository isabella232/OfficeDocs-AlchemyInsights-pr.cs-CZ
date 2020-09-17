---
title: Pracovní postup se nespouští
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794760"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="9372e-102">Pracovní postup se nespouští</span><span class="sxs-lookup"><span data-stu-id="9372e-102">Workflow is not starting</span></span>

- <span data-ttu-id="9372e-103">SharePoint 2010 a SharePoint 2013 pracovní postupy se nespouštějí.</span><span class="sxs-lookup"><span data-stu-id="9372e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="9372e-104">Pokud se váš pracovní postup nespouští, může se jednat o dočasný problém s poskytováním služeb, při kterém mohou uživatelé zaznamenat přerušované zpoždění pomocí pracovního postupu.</span><span class="sxs-lookup"><span data-stu-id="9372e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="9372e-105">Podívejte se na [řídicí panel stavu služeb](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) a zjistěte, jestli je vaše organizace ovlivněná.</span><span class="sxs-lookup"><span data-stu-id="9372e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="9372e-106">Pokud od prvního vystavení tohoto problému uplynulo více než 24 hodin, protokolujte lístek podpory.</span><span class="sxs-lookup"><span data-stu-id="9372e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9372e-107">V mnoha případech jsme na řešení ještě pracujeme.</span><span class="sxs-lookup"><span data-stu-id="9372e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9372e-108">Dokončete řešení alespoň 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="9372e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="9372e-109">Zpožděné zahájení pracovních postupů SharePoint 2010</span><span class="sxs-lookup"><span data-stu-id="9372e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="9372e-110">K tomu dojde, pokud je pracovní postup spuštěn ve velkých dávkách.</span><span class="sxs-lookup"><span data-stu-id="9372e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="9372e-111">(například když se přidají několik položek najednou)</span><span class="sxs-lookup"><span data-stu-id="9372e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="9372e-112">Pracovní postupy nejsou navržené pro spuštění v reálném čase, takže zpoždění se provádí podle chování.</span><span class="sxs-lookup"><span data-stu-id="9372e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="9372e-113">Pokud je pracovní postup komplexní jazyk XML (Extensible Object Markup Language), může být kompilace pomalé.</span><span class="sxs-lookup"><span data-stu-id="9372e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="9372e-114">Podívejte se na [Tento](https://support.microsoft.com//kb/3043697) článek.</span><span class="sxs-lookup"><span data-stu-id="9372e-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="9372e-115">Pracovní postup byste měli zjednodušit nebo ho přenavrhovat pomocí typu platformy Microsoft SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="9372e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="9372e-116">Pokud se vaše historie pracovního postupu zvětšila, můžete položky vymazat nebo vytvořit nový seznam historie.</span><span class="sxs-lookup"><span data-stu-id="9372e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="9372e-117">Další informace: [vymazání historie pracovního postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="9372e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="9372e-118">Související témata</span><span class="sxs-lookup"><span data-stu-id="9372e-118">Related topics</span></span>
<span data-ttu-id="9372e-119">Chcete vyzkoušet tok Microsoftu v SharePointu Online?</span><span class="sxs-lookup"><span data-stu-id="9372e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9372e-120">Vytvoření toku</span><span class="sxs-lookup"><span data-stu-id="9372e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9372e-121">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="9372e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


