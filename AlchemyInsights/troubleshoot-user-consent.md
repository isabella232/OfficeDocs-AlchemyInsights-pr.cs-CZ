---
title: Řešení potíží s souhlasem uživatele
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900959"
---
# <a name="troubleshoot-user-consent"></a>Řešení potíží s souhlasem uživatele

1. Můžete nakonfigurovat, jak budou koncoví uživatelé souhlasit s aplikacemi prostřednictvím portálu Azure nebo PowerShellu. Další informace najdete v článku [nastavení souhlasu uživatele](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Správce může také použít [rozhraní Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) k udělení souhlasu jménem jednoho uživatele. Další informace najdete v článku o [získání přístupu v zastoupení uživatele](https://docs.microsoft.com/graph/auth-v2-user).
1. [Chyby souhlasu uživatelů](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): Tento článek popisuje chyby, ke kterým může dojít při procesu přijetí do aplikace. Pokud chcete řešit potíže s neočekávanými zprávami o souhlasu, které neobsahují žádné chybové zprávy, přečtěte si článek [scénáře ověřování pro Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).