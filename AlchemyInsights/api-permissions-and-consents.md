---
title: Oprávnění a souhlas rozhraní API
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932090"
---
# <a name="api-permissions-and-consent"></a>Oprávnění a souhlas rozhraní API

Aplikace, které se integrují Microsoft identity platform a řídí se autorizačním modelem, který uživatelům a správcům umožňuje řídit přístup k datům. Implementace autorizačního modelu se aktualizovala na Microsoft identity platform koncového bodu. Změní způsob interakce aplikace s aplikací Microsoft identity platform. [Oprávnění a souhlas v koncovém Microsoft identity platform zahrnuje](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) základní koncepty tohoto modelu autorizace, včetně oborů, oprávnění a souhlasu.

Rozhraní [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) usnadňuje vývoj webových a nativních klientských aplikací s více tenanty. Tyto aplikace umožňují přihlášení podle uživatelských účtů z tenanta Azure AD, který se liší od těch, kde je aplikace registrovaná. Může také potřebovat přístup k webovým rozhraním API, jako je rozhraní Microsoft Graph API (pro přístup k Azure AD, Intune a službám v Microsoft 365) a dalším rozhraním API služby Microsoft kromě vlastních webových rozhraní API.

