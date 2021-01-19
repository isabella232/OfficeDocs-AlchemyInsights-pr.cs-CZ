---
title: Otázky týkající se souhlasu správce
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900931"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="8ed8c-102">Otázky týkající se souhlasu správce</span><span class="sxs-lookup"><span data-stu-id="8ed8c-102">Admin consent issues</span></span>

1. <span data-ttu-id="8ed8c-103">Povolte [pracovní postup souhlasu správce](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , aby uživatelé mohli požádat o schválení správcem přímo z obrazovky souhlasu.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="8ed8c-104">Pokud se vy nebo uživatelé vaší aplikace nezobrazují neočekávané chyby během souhlasu, podívejte se na tento článek: odstranění [souhlasu s aplikací – Neočekávaná chyba](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="8ed8c-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="8ed8c-105">Přečtěte si další informace o [souhlasu správce na platformě Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), o tom, jak funguje [výzva k souhlasu](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) a jak [vyhodnotit žádost o souhlas správy na úrovni tenanta](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="8ed8c-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="8ed8c-106">Aplikace, které integrují platformu Microsoft Identity Platform, sledují model autorizace, který uživatelům a správcům umožňuje ovládat způsob přístupu k datům.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="8ed8c-107">Implementace modelu autorizace byla aktualizována v koncovém bodě platformy Microsoft Identity Platform a změní způsob, jakým aplikace musí spolupracovat s platformou Microsoft identity.</span><span class="sxs-lookup"><span data-stu-id="8ed8c-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="8ed8c-108">Přehled tohoto modelu autorizace, včetně oborů, oprávnění a souhlasu, najdete [v tématu oprávnění a souhlas v koncovém bodě platformy Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .</span><span class="sxs-lookup"><span data-stu-id="8ed8c-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>