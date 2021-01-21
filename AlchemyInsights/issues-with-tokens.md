---
title: Problémy s tokeny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916738"
---
# <a name="issues-with-tokens"></a>Problémy s tokeny

Pokud chcete spravovat problémy související s tokeny, postupujte takto:

1. Můžete zadat dobu života Accessu, ID nebo tokenu SAML vystaveného společností Microsoft Identity Platform. Životnosti tokenů můžete nastavit pro všechny aplikace ve vaší organizaci, pro víceuživatelské (multi-Organization) aplikaci nebo pro konkrétní instanční objekt ve vaší organizaci. Další informace najdete v článku [Konfigurace životnosti tokenů v Microsoft Identity Platform (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Tokeny Accessu umožňují klientům bezpečně volat chráněné webové rozhraní API a využívají webové rozhraní API k ověřování a autorizaci. V rámci specifikace OAuth jsou tokeny Accessu neprůhledné řetězce bez nastaveného formátu – někteří poskytovatelé identit (IDPs) používají GUID, ostatní používají šifrované objekty blob. Microsoft Identity Platform používá různé formáty přístupových tokenů v závislosti na konfiguraci rozhraní API, které token přijímá. Informace o tom, jak může vaše rozhraní API ověřovat a používat deklarace v accessovém tokenu, najdete v tématu [Microsoft Identity Platform Access tokeny](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Knihovna Microsoft Authentication Library (MSAL) podporuje několik toků ověřování pro použití v různých scénářích aplikací. Další informace najdete v tématu [ověřování toků](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Autorizační kód OAuth 2,0 lze použít v aplikacích nainstalovaných na zařízení pro získání přístupu k chráněným prostředkům, jako jsou webová rozhraní API. Pomocí implementace OAuth 2,0 Microsoft Identity Platform můžete přidat přihlášení a přístup k rozhraní API k mobilním a desktopovým aplikacím. Informace o [toku autorizačního kódu Microsoft Identity Platform a OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) najdete v tématu jak program přímo oproti protokolu v aplikaci použít v jakémkoli jazyce.
5. OpenID Connect (OIDC) je protokol ověřování vytvořený na 2,0 OAuth, který můžete použít k bezpečnému přihlášení uživatele k aplikaci. Při použití implementace služby OpenID Connect v koncovém bodě platformy Microsoft Identity Platform můžete do aplikací přidat přihlášení a přístup k rozhraní API. [Protokol Microsoft Identity Platform and OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) ukazuje, jak to udělat nezávisle na jazyku a popisuje, jak odesílat a přijímat zprávy HTTP bez použití knihoven Microsoft Open-Source.
    - Koncový bod UserInfo je součástí standardu OIDC, který slouží k vrácení deklarací uživatele, který ověřil. Další informace najdete v tématu [Microsoft Identity Platform pro informace o uživateli](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Volání webového rozhraní API ve webové aplikaci pomocí Azure AD a OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) Sample ukazuje, jak vytvořit webovou aplikaci MVC, která používá Azure AD pro přihlášení pomocí protokolu OpenID Connect a potom volejte webové rozhraní API v rámci identity přihlášeného uživatele pomocí tokenů získaných prostřednictvím OAuth 2,0. V tomto příkladu se používá OpenID připojení k middlewaru OWIN a ADAL .NET .NET.
6. [Nakonfigurujte aplikaci tak, aby vystavila webové rozhraní API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – v tomto rychlým automatu zaregistrujete webové rozhraní API pomocí Microsoft Identity Platform a zpřístupníte ho klientským aplikacím přidáním příkladu oboru. Když zaregistrujete webové rozhraní API a vystavím ho prostřednictvím oborů, můžete k jeho prostředkům poskytnout přístup pomocí oprávnění autorizovaným uživatelům a klientským aplikacím, které mají přístup k rozhraní API.
7. V Azure Active Directory B2C (Azure AD B2C) je tok přihlašovacích údajů vlastníka prostředku (ROPC) standardní. V tomto toku aplikace, označovaná také jako předávající strana, si vymění platná pověření pro tokeny. Přihlašovací údaje zahrnují ID uživatele a heslo. Vrácené tokeny jsou tokeny ID, přístupový token a obnovovací token. Další informace najdete v článku [nastavení toku přihlašovacích údajů pro heslo vlastníka prostředků v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

