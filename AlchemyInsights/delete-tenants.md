---
title: Odstranit tenanta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564418"
---
# <a name="delete-tenant"></a>Odstranit tenanta

Pokud chcete odstranit Azure AD, zkontrolujte:
- Jste globálním správcem adresáře.
- Nejste přihlášeni pomocí účtu, který má výchozí adresář, jako je třeba contoso.onmicrosoft.com, v přihlášeném účtu, například admin@contoso.onmicrosoft.com.
- Před odstraněním odeberte všechny aktivní aplikace v adresáři. Pokud chcete odebrat aktivní aplikace, přejděte na registrace aplikací a odeberte stávající aplikace.
- Žádné aktivní předplatná pro žádné služby Microsoft Online Services, jako je Microsoft Azure, Office 365 nebo Azure AD Premium, přidružené k adresáři. Převeďte svoje předplatné nebo urychlení zrušení aktivních předplatných prostřednictvím podpory Azure a fakturace. Přečtěte si další informace o zrušení předplatného Office 365 a Azure. Pokyny k přidružení nebo přidání existujícího předplatného k tenantovi najdete v článku [přidružení nebo přidání předplatného Azure ke svému Tenantovi Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Žádná aktivní licence neexistuje. Pokud chcete licence odebrat, přečtěte si [článek Jak odebrat předplatné a odebrat licenci](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Při pokusu o odstranění Azure AD se v adresáři nevyskytují žádné další aktivní uživatele. Odeberte také všechny ostatní aktivní uživatele a všechny závislosti v názvu vlastní domény v klientovi budou rovněž odebrány, například uživatelé vytvoøeni pomocí admin@contoso.com.

Podrobnější pokyny:
- Odstranění "Azure Active Directory" nebo "předplatná", viz [odstranění služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Odebrání aplikací v adresáři: Přečtěte si článek [odebrání aplikací](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
