---
title: Oprávnění rozhraní API a proces souhlasu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404318"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="f49f5-102">Oprávnění rozhraní API a proces souhlasu</span><span class="sxs-lookup"><span data-stu-id="f49f5-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="f49f5-103">Aby vaše aplikace přistupovat k datům v Microsoft Graphu, musí mu uživatel nebo správce udělit správná oprávnění prostřednictvím procesu souhlasu.</span><span class="sxs-lookup"><span data-stu-id="f49f5-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="f49f5-104">[Odkaz na oprávnění aplikace Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) uvádí oprávnění přidružená ke každé hlavní sadě rozhraní Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="f49f5-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="f49f5-105">Obsahuje také pokyny k používání oprávnění.</span><span class="sxs-lookup"><span data-stu-id="f49f5-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="f49f5-106">**Nastavení nebo aktualizace hlavního objektu služby**</span><span class="sxs-lookup"><span data-stu-id="f49f5-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="f49f5-107">[Vytvoření objektu serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – tento článek ukazuje, jak vytvořit nový objekt servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="f49f5-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="f49f5-108">[Vytvoření](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) instančního objektu aplikace Azure AD & na portálu – tento článek vám ukáže, jak vytvořit novou aplikaci Azure Active Directory (Azure AD) a instanční objekt služby, který se může používat s řízením přístupu založeným na rolích.</span><span class="sxs-lookup"><span data-stu-id="f49f5-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="f49f5-109">[Aplikace &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) instanční objekty v Azure AD – tento článek popisuje registraci aplikací, aplikační objekty a objekty služby v Azure Active Directory: co jsou, jak se používají a jak se vzájemně souvisejí.</span><span class="sxs-lookup"><span data-stu-id="f49f5-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="f49f5-110">**Přidání nebo aktualizace registrace aplikací a poskytnutí souhlasu správce**</span><span class="sxs-lookup"><span data-stu-id="f49f5-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="f49f5-111">[Vytvoření registrace aplikace –](https://docs.microsoft.com/graph/api/application-post-applications) tento článek ukazuje, jak vytvořit nový objekt aplikace.</span><span class="sxs-lookup"><span data-stu-id="f49f5-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="f49f5-112">[Aktualizace registrace aplikace – oprávnění rozhraní API](https://docs.microsoft.com/graph/api/application-update) – tento článek ukazuje, jak aktualizovat vlastnosti objektu aplikace.</span><span class="sxs-lookup"><span data-stu-id="f49f5-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="f49f5-113">[Poskytnutí souhlasu správce](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – Pro souhlas správce a souhlas obecně požadujeme, aby správce výslovně udělí souhlas.</span><span class="sxs-lookup"><span data-stu-id="f49f5-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="f49f5-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – kontejner správy rolí pro jednotné definice rolí a přiřazení rolí pro poskytovatele Microsoft 365 RBAC, kteří podporují více objektů zabezpečení a více oborů v jednom přiřazení rolí.</span><span class="sxs-lookup"><span data-stu-id="f49f5-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="f49f5-115">Tento typ se liší od *typu zdroje rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="f49f5-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="f49f5-116">Příkladem takového poskytovatele RBAC je Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f49f5-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="f49f5-117">Přiřazení rolí v Intune může mít matici objektů zabezpečení a matici skupin oborů.</span><span class="sxs-lookup"><span data-stu-id="f49f5-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="f49f5-118">**To je v beta verzi, což znamená, že je stále ve vývoji a nedoporučuje se používat v produkční verzi.**</span><span class="sxs-lookup"><span data-stu-id="f49f5-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
