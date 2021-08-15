---
title: Odstranění tenanta
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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993886"
---
# <a name="delete-tenant"></a>Odstranění tenanta

Pokud chcete odstranit Azure AD, ujistěte se, že:
- Jste globální správce v adresáři.
- Nejste přihlášení pomocí účtu, který má výchozí adresář, například contoso.onmicrosoft.com v účtu přihlášení, například pomocí admin@contoso.onmicrosoft.com.
- Před odstraněním odeberte všechny aktivní aplikace v adresáři. Pokud chcete odebrat aktivní aplikace, přejděte na Registrace aplikací a odeberte stávající aplikace.
- Nejsou k dispozici žádná aktivní předplatná pro žádné služby Microsoft Online Services, jako Microsoft Azure, Office 365 nebo Azure AD Premium přidružené k adresáři. Přeneste si předplatná nebo urychlete zrušení aktivních předplatných prostřednictvím podpory a fakturace Azure. Přečtěte si další informace o zrušení předplatného Office 365 a předplatných Azure. Pokyny k přidružení nebo přidání stávajícího předplatného k tenantovi najdete v tématu Přidružení nebo přidání předplatného Azure do [tenanta Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Neexistuje žádná aktivní licence. Pokud chcete odebrat licence, podívejte se na postup odebrání [předplatného k odebrání licence.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Při pokusu o odstranění Azure AD nejsou v adresáři kromě sebe jako globální správce žádní další aktivní uživatelé. Odeberte všechny ostatní aktivní uživatele a všechny závislosti na vlastním názvu domény v tenantovi se taky budou muset odebrat, například uživatelé, kteří vytvořili admin@contoso.com.

Další podrobnosti o tom, jak:
- Odstraňte "Azure Active Directory" nebo "předplatné", viz [Odstranění Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Odebrání aplikací v adresáři najdete v tématu [Odebrání aplikací](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
