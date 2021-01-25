---
title: Problém zřizování SCIM
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949712"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="0fbc2-102">Problém zřizování SCIM</span><span class="sxs-lookup"><span data-stu-id="0fbc2-102">SCIM provisioning issue</span></span>

<span data-ttu-id="0fbc2-103">Automatické zřizování odkazuje na vytváření uživatelských identit a rolí v cloudových aplikacích, ke kterým potřebují uživatelé přístup.</span><span class="sxs-lookup"><span data-stu-id="0fbc2-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="0fbc2-104">Kromě vytváření identit uživatelů zahrnuje Automatické zřizování správu a odebrání identit uživatelů jako stavu nebo změny rolí.</span><span class="sxs-lookup"><span data-stu-id="0fbc2-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="0fbc2-105">Než začnete s nasazením, můžete zkontrolovat, [jak zřizování funguje](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) , aby se zjistilo, jak zřizování Azure Active Directory (AD) funguje, a získejte doporučení pro konfiguraci.</span><span class="sxs-lookup"><span data-stu-id="0fbc2-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="0fbc2-106">Jako vývojář aplikací můžete použít rozhraní API pro správu uživatelů pro různé domény (SCIM), které umožňuje automatické zřizování uživatelů a skupin mezi aplikací a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0fbc2-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="0fbc2-107">[Vytvoření koncového bodu SCIM a konfigurace zřizování uživatelů pomocí služby Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) popisuje, jak vytvořit SCIM koncový bod a integrovat ho se službou Azure AD zřizování.</span><span class="sxs-lookup"><span data-stu-id="0fbc2-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



