---
title: Problémy se souhlasem správce
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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952566"
---
# <a name="admin-consent-issues"></a>Problémy se souhlasem správce

1. Povolte [pracovní postup souhlasu správce,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) aby uživatelé žádat o schválení správcem přímo z obrazovky souhlasu.

1. Pokud se vám nebo uživatelům vaší aplikace během procesu souhlasu zobrazí neočekávané chyby, podívejte se na tento článek s pokyny k řešení potíží: Neočekávaná chyba při provádění souhlasu s [aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Přečtěte si další informace [o souhlasu správce na Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), o tom, jak funguje výzva k souhlasu a jak vyhodnotit žádost o souhlas správce pro celou [tenanta](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent). [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)

1. Aplikace, které se integrují Microsoft identity platform a řídí se autorizačním modelem, který uživatelům a správcům umožňuje řídit přístup k datům. Implementace autorizačního modelu se aktualizovala v koncovém Microsoft identity platform a mění způsob interakce aplikace s Microsoft identity platform. Přehled [tohoto modelu autorizace,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) včetně oborů, oprávnění a souhlasu, najdete v článku Oprávnění a souhlas v koncovém Microsoft identity platform.