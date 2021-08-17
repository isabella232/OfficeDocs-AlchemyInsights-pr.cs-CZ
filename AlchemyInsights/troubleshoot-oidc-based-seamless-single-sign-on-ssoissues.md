---
title: Řešení potíží s bezproblémovým jednotným přihlašováním (SSO) založeným na OIDC
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105761"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Řešení potíží s bezproblémovým jednotným přihlašováním (SSO) založeným na OIDC

- Informace o tom, jak přidat aplikaci založenou na OIDC do tenanta Azure, najdete v tématu Rychlý start: Nastavení jednotného přihlašování [(SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)založeného na OIDC pro aplikaci v tenantovi Azure Active Directory (Azure AD).
- Další informace o aplikacích, které používají standard OpenID Připojení k implementaci jednotného přihlašování, najdete v tématu Principy jednotného přihlašování založeného na [OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Informace pro případ, že se rozhodnete napsat svůj kód přímo odesláním a zpracováním požadavků HTTP nebo použitím open-source knihovny třetích stran, místo použití jedné z našich open-source knihoven, najdete v článku [Protokoly OAuth 2.0 a OpenID Připojení](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)na Microsoft identity platform .

**Protokoly**

1. [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) a implicitní tok udělení – Určující charakteristikou implicitního grantu je, že tokeny (tokeny ID nebo přístupové tokeny) jsou vráceny přímo z koncového bodu /authorize místo koncového bodu /token. Tento kód se často používá jako součást toku autorizačního kódu, který se nazývá **"hybridní tok" –** načtení tokenu ID v žádosti /authorize spolu s autorizačním kódem . Tento článek popisuje, jak naprogramovat přímo proti protokolu ve vaší aplikaci a požádat o tokeny z Azure AD.
2. Microsoft identity platform a [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Udělení autorizačního kódu OAuth 2.0 můžete použít v aplikacích nainstalovaných na zařízení k získání přístupu k chráněným prostředkům, jako jsou webová rozhraní API. Pomocí Microsoft identity platform OAuth 2.0 můžete přidat přihlášení a přístup k rozhraní API do mobilních a **desktopových aplikací.** Tento článek popisuje, jak programovat přímo proti protokolu v aplikaci pomocí libovolného jazyka.
3. Microsoft identity platform a [OpenID Připojení](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Když použijete implementaci OpenID Připojení Microsoft identity platform Microsoft identity platform, můžete do svých aplikací přidat přihlášení a přístup k rozhraní API. Tento článek popisuje, jak to udělat nezávisle na jazyce a popisuje, jak odesílat a přijímat zprávy HTTP bez **použití open-source** knihoven Microsoftu.
4. Microsoft identity platform a tok přihlašovacích údajů klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Pro přístup k prostředkům hostovaným na webu pomocí identity aplikace můžete použít udělení klientských přihlašovacích údajů OAuth 2.0 zadané v dokumentu RFC 6749, někdy nazývané dvounohé **OAuth.** Tento typ grantu se běžně používá pro interakce mezi serverem, které musí běžet na pozadí bez okamžité interakce s uživatelem. Tyto typy aplikací se často označují jako **démony** nebo **účty služeb**. Tento článek popisuje, jak programovat přímo proti protokolu v aplikaci.
