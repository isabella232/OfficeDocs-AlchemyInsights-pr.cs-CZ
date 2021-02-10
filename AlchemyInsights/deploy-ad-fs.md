---
title: Nasazení služby AD FS
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177441"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="a86f8-102">Nasazení služby AD FS</span><span class="sxs-lookup"><span data-stu-id="a86f8-102">Deploy AD FS</span></span>

<span data-ttu-id="a86f8-103">Nasazení služby AD FS (Active Directory Federation Services) používá k ověření uživatelů ve službách Office 365 vaši místní infrastrukturu.</span><span class="sxs-lookup"><span data-stu-id="a86f8-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="a86f8-104">Federovaným přihlášením můžete uživatelům povolit přihlášení ke službám Office 365 a softwaru jako službě (SAAS), které jsou integrované s Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a86f8-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="a86f8-105">Federované přihlašování ověřuje uživatele ve vaší místní službě Active Directory prostřednictvím AD FS.</span><span class="sxs-lookup"><span data-stu-id="a86f8-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="a86f8-106">V podnikové síti navíc uživatelé nebudou mít k opětovnému zadání hesla potřebná k zadání hesla.</span><span class="sxs-lookup"><span data-stu-id="a86f8-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="a86f8-107">Poradce [pro nasazení SLUŽBY AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) vám poskytne podrobné pokyny k nasazení místní infrastruktury AD FS, která ověřuje uživatele ve službách Microsoft 365 a Office 365.</span><span class="sxs-lookup"><span data-stu-id="a86f8-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="a86f8-108">V této příručce může vaše organizace zkontrolovat komponenty a požadavky služby AD FS, získat a nainstalovat certifikáty SSL, které jsou nezbytné pro nasazení, a nainstalovat požadovaný proxy server webových aplikací.</span><span class="sxs-lookup"><span data-stu-id="a86f8-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
