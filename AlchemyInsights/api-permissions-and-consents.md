---
title: Oprávnění a souhlas s rozhraním API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974374"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="c0b2f-102">Oprávnění a souhlas s rozhraním API</span><span class="sxs-lookup"><span data-stu-id="c0b2f-102">API permissions and consent</span></span>

<span data-ttu-id="c0b2f-103">Aplikace, které integrují platformu Microsoft Identity Platform, sledují model autorizace, který uživatelům a správcům umožňuje ovládat způsob přístupu k datům.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="c0b2f-104">Implementace modelu autorizace byla aktualizována na koncovém bodu Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="c0b2f-105">Změní se způsob interakce aplikace s platformou Microsoft identity.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="c0b2f-106">[Oprávnění a souhlas v koncovém bodě platformy Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) pokrývá základní koncepty tohoto modelu autorizace, včetně oborů, oprávnění a souhlasu.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="c0b2f-107">[Souhlasní rámec služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) usnadňuje vývoj webových a nativních klientských aplikací pro více tenantů.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="c0b2f-108">Tyto aplikace umožňují přihlásit se uživatelskými účty z Azure AD tenanta, který se liší od toho, odkud je aplikace registrovaná.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="c0b2f-109">Mohou také potřebovat přístup k webovým rozhraním API, jako je Microsoft Graph API (pro přístup k Azure AD, Intune a službám v Microsoft 365) a dalším rozhraním API služeb Microsoftu, a to kromě vlastních webových rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="c0b2f-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

