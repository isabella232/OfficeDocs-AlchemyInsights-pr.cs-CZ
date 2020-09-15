---
title: Aktivace chybějícího pracovního postupu se nezdařila
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667079"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="7e1f3-102">Aktivace chybějícího pracovního postupu se nezdařila</span><span class="sxs-lookup"><span data-stu-id="7e1f3-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="7e1f3-103">V kolekci webů Microsoft SharePointu nelze do seznamu nebo knihovny přidat globálně opakovaně použitelný pracovní postup (například schválení – SharePoint 2010 ").</span><span class="sxs-lookup"><span data-stu-id="7e1f3-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="7e1f3-104">Tento problém vyřešíte takto:</span><span class="sxs-lookup"><span data-stu-id="7e1f3-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="7e1f3-105">Otevřete kořenový web kolekce webů v SharePoint designeru 2013.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="7e1f3-106">V části **objekty webu**vyberte **pracovní postupy**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="7e1f3-107">V části **Nový** na pásu karet **pracovní postupy** vyberte **opakovaně použitelný pracovní postup**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="7e1f3-108">Ve formuláři **vytvořit opakovaně použitelný pracovní postup** zadejte název \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="7e1f3-109">V nabídce **typ platformy**klikněte na **pracovní postup SharePointu 2010**a potom klikněte na **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="7e1f3-110">V části **Uložit** na pásu karet **pracovního postupu** vyberte **publikovat**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="7e1f3-111">V části **Spravovat** na pásu karet **pracovního postupu** vyberte **publikovat globálně**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="7e1f3-112">V potvrzovacím dialogovém okně, které se zobrazí, vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="7e1f3-113">Ve webovém prohlížeči přejděte na kořenový web kolekce webů a potom na **Site Settings** \> **funkce kolekce webů**nastavení aplikace Access.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="7e1f3-114">Potom přepněte funkci **pracovní postupy** :</span><span class="sxs-lookup"><span data-stu-id="7e1f3-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="7e1f3-115">· Pokud je tato funkce  *aktivovaná*  , klikněte na **deaktivovat** a potom na **aktivovat**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="7e1f3-116">· Pokud je tato funkce  *Deaktivovaná*  , klikněte na **aktivovat**.</span><span class="sxs-lookup"><span data-stu-id="7e1f3-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="7e1f3-117">Další informace najdete v následujícím [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="7e1f3-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

