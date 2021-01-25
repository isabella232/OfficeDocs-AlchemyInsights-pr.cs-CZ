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
# <a name="api-permissions-and-consent"></a>Oprávnění a souhlas s rozhraním API

Aplikace, které integrují platformu Microsoft Identity Platform, sledují model autorizace, který uživatelům a správcům umožňuje ovládat způsob přístupu k datům. Implementace modelu autorizace byla aktualizována na koncovém bodu Microsoft Identity Platform. Změní se způsob interakce aplikace s platformou Microsoft identity. [Oprávnění a souhlas v koncovém bodě platformy Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) pokrývá základní koncepty tohoto modelu autorizace, včetně oborů, oprávnění a souhlasu.

[Souhlasní rámec služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) usnadňuje vývoj webových a nativních klientských aplikací pro více tenantů. Tyto aplikace umožňují přihlásit se uživatelskými účty z Azure AD tenanta, který se liší od toho, odkud je aplikace registrovaná. Mohou také potřebovat přístup k webovým rozhraním API, jako je Microsoft Graph API (pro přístup k Azure AD, Intune a službám v Microsoft 365) a dalším rozhraním API služeb Microsoftu, a to kromě vlastních webových rozhraní API.

