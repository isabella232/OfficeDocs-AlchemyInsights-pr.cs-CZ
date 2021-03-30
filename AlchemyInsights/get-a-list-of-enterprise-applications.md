---
title: Získání seznamu podnikových aplikací
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404331"
---
# <a name="get-a-list-of-enterprise-applications"></a>Získání seznamu podnikových aplikací

1. Seznam **podnikových** aplikací (všechny aplikace nebo filtrované podle zobrazovaných názvů, ID, identifikátorů URI identifikátorů atd.) pomocí příkazu Powershellu najdete v tématu [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Seznam hlavních objektů služby (všechny objekty nebo filtrované podle ID) pomocí příkazu Powershellu najdete v tématu [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Pokud chcete získat **seznam aplikací konfigurovaných samlem, můžou** vám pomoct následující skripty PowerShellu:

    Každá aplikace, ať už je to aplikace OAuth nebo aplikace SAML (galerie i aplikace mimo galerii), by měly v AAD při registraci vytvořeny dva objekty. Jeden z nich se nazývá Objekt aplikace a druhý objekt Hlavní služba. Když vysypáte vlastnosti hlavního objektu služby pomocí PowerShellu, zjistíte, že každá aplikace má určitý počet značek, které jsou s ním spojené, třeba:

    - Aplikace OAuth budou mít značku s názvem **WindowsAzureActiveDirectoryIntegratedApp.**
    - Galerie aplikací SAML by měl značku s názvem **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**
    - Aplikace SAML, které nejsou v galerii, by vlastnily značku s názvem **WindowsAzureActiveDirectoryCustomSingleSignOnApplication.**

    Proto můžete tyto značky použít a zjistit, jaký druh aplikace to je. Značka **WindowsAzureActiveDirectoryIntegratedApp je** společná pro všechny typy aplikací. Následující výstřižek kódu můžete použít k zobrazení seznamu všech aplikací SAML (v galerii i mimo galerii):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Další informace najdete v tématu Určení aplikací [s podporou SAML ve službě Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Vyhledání a seznam jenom webových aplikací:** Pomocí následujícího příkazu můžete získat všechny aplikace Azure AD s typem aplikace "Web app/API".

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Vyhledání a seznam samotných nativních aplikací:** Spuštěním následujícího příkazu získáte všechny nativní klientské aplikace (desktopové nebo mobilní zařízení).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Export všech registrovaných podrobností aplikace Azure AD** do formátu CSV: Následující příkaz exportuje všechny aplikace Azure AD s požadovanými podrobnostmi do souboru CSV:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Potřebujete exportovat seznam nepoužívaných aplikací Azure** – sestava auditování

    Azure AD může zobrazovat protokoly aplikací jenom po dobu 30 dnů za předpokladu, že máte licenci Azure AD Premium.
    Data můžete uchovávat po dobu delší než 30 dnů. Pomocí rozhraní [API pro vytváření sestav Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) můžete data načíst programově a ukládat je do databáze. Protokoly auditování můžete také integrovat do systému SIEM třetí strany.

    Můžete si taky stáhnout seznam aplikací pro všechny aplikace a vlastněné aplikace v části Azure Active directory>Registrace aplikací>Stáhnout>Všechny aplikace/Vlastněné aplikace.

    Seznam aplikací přes MS Graph najdete v tématu Seznam aplikací [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) a typ prostředku [aplikace – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
