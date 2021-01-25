---
title: Mapování atributů pro zřizování uživatelů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949666"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="5a43f-102">Mapování atributů pro zřizování uživatelů</span><span class="sxs-lookup"><span data-stu-id="5a43f-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="5a43f-103">Informace o řešení známých problémů s mapováním atributů najdete v tématu [mapování atributů](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="5a43f-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="5a43f-104">Microsoft Azure Active Directory (AD) poskytuje podporu pro zřizování uživatelů pro aplikace SaaS třetích stran, jako jsou Salesforce, G Suite a další.</span><span class="sxs-lookup"><span data-stu-id="5a43f-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="5a43f-105">Pokud povolíte zřizování uživatelů pro aplikaci SaaS pro třetí strany, portál Azure ho řídí jeho hodnoty atributů prostřednictvím mapování atributů.</span><span class="sxs-lookup"><span data-stu-id="5a43f-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="5a43f-106">Informace o tom, jak přizpůsobit výchozí mapování atributů, najdete v tématu [přizpůsobení atributu zřizování uživatelů – mapování pro aplikace SaaS v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="5a43f-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="5a43f-107">Další informace o zřizování uživatelů aplikace pro SaaS najdete v tématu [co je automatizované zřizování aplikací aplikace SaaS v Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="5a43f-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="5a43f-108">Při přizpůsobení mapování atributů pro zřizování uživatelů se může stát, že se atribut, který chcete mapovat, nezobrazí v seznamu zdrojových atributů.</span><span class="sxs-lookup"><span data-stu-id="5a43f-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="5a43f-109">[Synchronizace atributu z vaší místní služby Active Directory do služby Azure AD pro zřizování](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) v článku aplikace vám ukáže, jak přidat chybějící atribut tím, že ho synchronizuje z vaší místní služby AD s Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a43f-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
