---
title: Sdílení s externími uživateli nefunguje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691568"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="9e852-102">Řešení problémů se sdílením obsahu služby SharePoint s externími uživateli</span><span class="sxs-lookup"><span data-stu-id="9e852-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="9e852-103">Ujistěte se, že je ve vaší organizaci zapnuté externí sdílení:</span><span class="sxs-lookup"><span data-stu-id="9e852-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="9e852-104">Přejděte na [ &amp; stránku doplňky služeb v centru pro správu Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a klikněte na **weby**.</span><span class="sxs-lookup"><span data-stu-id="9e852-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="9e852-105">Zkontrolujte, jestli je nastavení zapnuté.</span><span class="sxs-lookup"><span data-stu-id="9e852-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="9e852-106">Pokud je vybraná možnost jenom stávající externí uživatelé, zkontrolujte, jestli je externí uživatel uvedený v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9e852-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="9e852-107">Zkontrolujte, jestli je na webu zapnuté externí sdílení.</span><span class="sxs-lookup"><span data-stu-id="9e852-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="9e852-108">Pro klasickou kolekci webů:</span><span class="sxs-lookup"><span data-stu-id="9e852-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="9e852-109">V novém centru pro správu SharePointu v levém podokně klikněte na **weby**.</span><span class="sxs-lookup"><span data-stu-id="9e852-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="9e852-110">Vyberte web nebo weby a na pásu karet klikněte na **sdílení**.</span><span class="sxs-lookup"><span data-stu-id="9e852-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="9e852-111">Pro týmový web, který patří do skupiny Microsoft 365 nebo komunikační web:</span><span class="sxs-lookup"><span data-stu-id="9e852-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="9e852-112">Tyto nové typy webů mají stejné nastavení sdílení jako nastavení pro celou organizaci, pokud toto nastavení neumožňuje sdílení souborů pomocí odkazů, které nevyžadují přihlášení.</span><span class="sxs-lookup"><span data-stu-id="9e852-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="9e852-113">V tomto případě weby povolí sdílení s novými a stávajícími externími uživateli, kteří se přihlásí.</span><span class="sxs-lookup"><span data-stu-id="9e852-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="9e852-114">Pokud chcete změnit nastavení pro určité weby, použijte nové centrum pro správu SharePointu nebo PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9e852-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="9e852-115">[Další informace](https://go.microsoft.com/fwlink/?linkid=871863)</span><span class="sxs-lookup"><span data-stu-id="9e852-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="9e852-116">Nastavení externího sdílení libovolného webu může být více omezující než vaše nastavení pro celou organizaci, ale neomezenější než u celé organizace.</span><span class="sxs-lookup"><span data-stu-id="9e852-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

