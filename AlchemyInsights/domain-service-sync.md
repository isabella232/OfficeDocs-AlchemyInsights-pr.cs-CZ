---
title: Synchronizace doménové služby
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884955"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="b0135-102">Synchronizace doménové služby</span><span class="sxs-lookup"><span data-stu-id="b0135-102">Domain service synchronization</span></span>

<span data-ttu-id="b0135-103">Objekty a přihlašovací údaje ve spravované doméně služby Azure Active Directory Domain Services (Azure AD DS) se dají vytvářet místně v doméně nebo jsou synchronizované z tenanta služby Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b0135-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="b0135-104">Při prvním nasazení Azure AD DS je nakonfigurována Automatická Jednosměrná synchronizace a replikuje objekty z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0135-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="b0135-105">Tato Jednosměrná synchronizace pokračuje v provozu na pozadí, aby byla k disběhové doméně spravované Azure AD DS se všemi změnami z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0135-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="b0135-106">Z Azure AD DS se nesynchronizuje žádná synchronizace na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0135-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="b0135-107">Další podrobnosti o synchronizaci doménové služby Azure Active Directory najdete v tématu [synchronizace doménové služby](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="b0135-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
