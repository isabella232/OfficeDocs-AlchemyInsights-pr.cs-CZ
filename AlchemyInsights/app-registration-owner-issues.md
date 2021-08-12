---
title: Problémy s vlastníkem registrace aplikací
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951126"
---
# <a name="app-registration-owner-issues"></a>Problémy s vlastníkem registrace aplikací

Tady jsou dostupné metody pro přidání objektů zabezpečení jako vlastníků pro registrace aplikací:

- Použití modulu Azure AD PowerShell –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Používání Azure CLI – `az ad app owner add`

    Reference: [vlastník aplikace az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Použití ms Graph -

    Reference: [Přidání vlastníka – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Použití portálu Azure AD Portal – přejděte na [portal.azure.com](https://portal.azure.com/) > Azure Active directory > Registrace aplikací > Vyberte aplikaci > Vlastníci > Přidat vlastníky

**Nemůžete zobrazit vaši aplikaci v okně Registrace aplikací, i když jste vlastníkem této aplikace?**

Vlastníkem aplikace není role správce. Pokud je povolené nastavení Omezit přístup k portálu pro správu [Azure AD,](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) bude moct aplikace na portálu registrace aplikací zobrazit jenom správce. Aby mohl vlastník zobrazit aplikace, zakažte toto nastavení (Nastavte to na NE) nebo přiřaďte roli správce vlastníkovi jenom pro konkrétní aplikaci. K tomu ale budete potřebovat Azure AD Premium P2 licenci a povolit [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
