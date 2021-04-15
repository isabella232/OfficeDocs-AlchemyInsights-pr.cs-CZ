---
title: Synchronizace 4Dhod je zakázaná.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782144"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="08c13-102">Synchronizace 4Dhod je zakázaná.</span><span class="sxs-lookup"><span data-stu-id="08c13-102">UPN sync disabled</span></span>

<span data-ttu-id="08c13-103">Pokud jste začali synchronizovat s Azure AD před 30. březnem 2016, spusťte následující rutinu Azure AD PowerShell, abyste povolovali soft match upn jenom pro vaši organizaci:</span><span class="sxs-lookup"><span data-stu-id="08c13-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="08c13-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="08c13-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="08c13-105">Automatická shoda upn se automaticky zapne pro organizace, které začaly synchronizovat s Azure AD 30. března 2016 nebo po tomto datu.</span><span class="sxs-lookup"><span data-stu-id="08c13-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="08c13-106">Další informace o povolení měkké shody v upn a dalších funkcích synchronizace najdete v tématu [Funkce synchronizační](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)služby Azure AD Connect .</span><span class="sxs-lookup"><span data-stu-id="08c13-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

