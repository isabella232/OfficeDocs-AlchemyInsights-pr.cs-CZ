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
# <a name="admin-consent-issues"></a>Otázky týkající se souhlasu správce

1. Povolte [pracovní postup souhlasu správce](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , aby uživatelé mohli požádat o schválení správcem přímo z obrazovky souhlasu.

1. Pokud se vy nebo uživatelé vaší aplikace nezobrazují neočekávané chyby během souhlasu, podívejte se na tento článek: odstranění [souhlasu s aplikací – Neočekávaná chyba](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Přečtěte si další informace o [souhlasu správce na platformě Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), o tom, jak funguje [výzva k souhlasu](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) a jak [vyhodnotit žádost o souhlas správy na úrovni tenanta](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplikace, které integrují platformu Microsoft Identity Platform, sledují model autorizace, který uživatelům a správcům umožňuje ovládat způsob přístupu k datům. Implementace modelu autorizace byla aktualizována v koncovém bodě platformy Microsoft Identity Platform a změní způsob, jakým aplikace musí spolupracovat s platformou Microsoft identity. Přehled tohoto modelu autorizace, včetně oborů, oprávnění a souhlasu, najdete [v tématu oprávnění a souhlas v koncovém bodě platformy Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .