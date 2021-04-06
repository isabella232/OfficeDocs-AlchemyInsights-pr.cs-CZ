---
title: Zjištění problémů s virtuálním desktopem Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595512"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="b8a4f-102">Zjištění problémů s virtuálním desktopem Windows</span><span class="sxs-lookup"><span data-stu-id="b8a4f-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="b8a4f-103">Windows Virtual Desktop Diagnostics používá jenom jednu rutinu PowerShellu, ale obsahuje mnoho volitelných parametrů, které pomáhají zúžit a izolovat problémy.</span><span class="sxs-lookup"><span data-stu-id="b8a4f-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="b8a4f-104">Začínáme:</span><span class="sxs-lookup"><span data-stu-id="b8a4f-104">To get started:</span></span> 

1. <span data-ttu-id="b8a4f-105">Stáhněte a naimportujte modul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b8a4f-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="b8a4f-106">Podrobnosti najdete v tématu [Rutiny virtuální plochy Windows pro Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="b8a4f-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="b8a4f-107">Přihlaste se ke svému účtu spuštěním následující rutiny:</span><span class="sxs-lookup"><span data-stu-id="b8a4f-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="b8a4f-108">Příklad: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="b8a4f-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="b8a4f-109">**POZNÁMKA:** Všechny dotazy používající PowerShell musí obsahovat parametry -UserName nebo -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="b8a4f-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="b8a4f-110">Informace o možnostech monitorování najdete v tématu Použití [analýzy protokolů pro funkci diagnostiky.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="b8a4f-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="b8a4f-111">Pokud chcete filtrovat diagnostické aktivity podle uživatele, spusťte následující rutinu:</span><span class="sxs-lookup"><span data-stu-id="b8a4f-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="b8a4f-112">Příklad: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="b8a4f-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="b8a4f-113">Existuje seznam filtrů, které můžete spustit, abyste diagnostikovali problémy.</span><span class="sxs-lookup"><span data-stu-id="b8a4f-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="b8a4f-114">Další informace o diagnostice problémů najdete v tématu Určení a diagnostika problémů s [virtuálním desktopem Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="b8a4f-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="b8a4f-115">Další informace o běžných chybách najdete v tématu [Běžné chyby senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="b8a4f-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
