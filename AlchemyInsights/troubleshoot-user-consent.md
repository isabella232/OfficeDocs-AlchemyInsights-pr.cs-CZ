---
title: Poradce při potížích se souhlasem uživatele
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
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007891"
---
# <a name="troubleshoot-user-consent"></a>Poradce při potížích se souhlasem uživatele

1. Způsob souhlasu koncových uživatelů s aplikacemi můžete nakonfigurovat prostřednictvím portálu Azure Portal nebo PowerShellu. Další [informace najdete v článku Nastavení souhlasu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) uživatelů.
1. Správce může také použít rozhraní [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) k udělení souhlasu s delegovaná oprávněními jménem jednoho uživatele. Další informace najdete v tématu [Získání přístupu jménem uživatele](https://docs.microsoft.com/graph/auth-v2-user).
1. [Chyby souhlasu uživatele:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)Tento článek popisuje chyby, ke kterým může dojít během procesu souhlasu s aplikací. Pokud řešení potíží s neočekávanými výzvami k souhlasu, které neobsahují žádné chybové zprávy, najdete v tématu Scénáře ověřování [pro Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).