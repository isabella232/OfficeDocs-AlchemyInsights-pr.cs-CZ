---
title: Chyby aplikace
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931442"
---
# <a name="application-errors"></a>Chyby aplikace

Hledáte informace o kódech **chyb AADSTS** vrácených ze služby tokenů zabezpečení (STS) Azure Active Directory (Azure AD)? Přečtěte [si kódy chyb ověřování](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) a autorizace Azure AD a vyhledejte popisy chyb AADSTS, opravy a některá navrhovaná alternativní řešení.

Chyby autorizace mohou být výsledkem několika různých problémů, z nichž většina vygeneruje chybu 401 nebo 403. K chybám autorizace může například vést následující:

- Nesprávné [toky akvizice přístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Špatně nakonfigurované [rozsahy oprávnění](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Chybějící [souhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Pokud chcete vyřešit běžné chyby autorizace, vyzkoušejte níže uvedené kroky, které nejvíce odpovídají chybě, kterou dostáváte. Může se použít více než jedna.

**401 Unauthorized error: Is your token valid?** (401 Chyba autorizace: Máte platný token?)

Ujistěte se, že vaše aplikace prezentuje platný přístupový token pro Microsoft Graph jako součást žádosti. Tato chyba často znamená, že v záhlaví žádosti o ověření protokolu HTTP chybí přístupový token, že je token neplatný nebo že vypršela jeho platnost. Důrazně doporučujeme použít knihovnu [MSAL (Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) pro získání přístupových tokenů. K této chybě může dojít také v případě, že se pokusíte použít delegovaný přístupový token udělený osobnímu účtu Microsoft pro přístup k rozhraní API, které podporuje jenom pracovní nebo školní účty (účty organizace).

**403 Forbidden error: Have you chosen the right set of permissions?** (chyba 403 Zakázáno: Vybrali jste správnou sadu oprávnění?)

Zkontrolujte, jestli jste požádali o správnou sadu oprávnění na základě rozhraní Microsoft Graph api pro volání aplikací. Doporučená nejméně privilegovaná oprávnění jsou k dispozici ve všech tématech referenční metody rozhraní Microsoft Graph API. Tato oprávnění musí navíc aplikaci udělit uživatel nebo správce. Udělení oprávnění obvykle probíhá prostřednictvím stránky souhlasu nebo udělením oprávnění pomocí okna registrace aplikace Azure Portal. V okně **Nastavení** aplikace klikněte na **Povinná oprávnění** a potom na **Udělit oprávnění**.

- [Oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference) 
- [Principy oprávnění a souhlasu v Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Forbidden error: Did your app acquire a token to match chosen permissions?** (chyba 403 Zakázáno: Získala vaše aplikace token odpovídající vybraným oprávněním?)

Ujistěte se, že typ požadovaných nebo udělených oprávnění odpovídá typu přístupového tokenu, který vaše aplikace získá. Možná požadujete a udělujíte oprávnění aplikací, ale místo tokenů toku klientských přihlašovacích údajů používáte delegované tokeny toku interaktivního kódu nebo požadujete a udělují delegovaná oprávnění, ale místo tokenů toku delegovaného kódu používáte tokeny toku přihlašovacích údajů klienta.

- [Získání přístupu jménem uživatelů a delegovaná oprávnění](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – tok autorizačního kódu OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získání přístupu bez oprávnění pro uživatele (služba proces démona) a aplikace](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – tok přihlašovacích údajů klienta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Forbidden error: Resetting password** (chyba 403 Zakázáno: Resetování hesla)

V současné době neexistují žádná oprávnění typu služba-služba pro oprávnění aplikací procesu démona, která by umožnila resetování uživatelských hesel. Tato rozhraní API jsou podporovaná jenom přes delegované interaktivní toky kódu s přihlášeným správcem.

- [Oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference)

**403 Forbidden: Does the user have access and are they licensed?** (403 Zakázáno: Má uživatel přístup a licenci?)

U toků delegovaného kódu microsoft Graph, jestli je žádost povolená na základě oprávnění udělených aplikaci a oprávnění, která má přihlášený uživatel. Tato chyba obecně znamená, že uživatel nemá dostatečná oprávnění k provedení žádosti nebo nemá licenci pro přístup k požadovaným datům. Žádost můžou úspěšně provést jenom uživatelé s požadovanými oprávněními nebo licencemi.

**403 Forbidden: Did you select the correct resource API?** (403 Zakázáno: Vybrali jste správné rozhraní API prostředku?)

Služby ROZHRANÍ API, jako je Microsoft Graph, kontrolují, že deklarace aud (cílová skupina) v přijatém přístupového tokenu odpovídá hodnotě, kterou očekává sama o sobě, a pokud ne, výsledkem je chyba 403 Zakázáno. Běžný omyl, který vede k této chybě, je použití tokenu získaného pro rozhraní API Azure AD Graphu, rozhraní API Outlooku nebo rozhraní API SharePointu/OneDrivu k volání Microsoft Graphu (nebo naopak). Ujistěte se, že prostředek (nebo obor), pro který vaše aplikace získává token, odpovídá rozhraní API, které aplikace volá.

**400 Bad Request / 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?** (400 Nesprávná žádost / 403 Zakázáno: Splňuje uživatel zásady podmíněného přístupu organizace (CA)?)

Na základě zásad certifikační autority organizace může být uživatel, který přistupuje k prostředkům Microsoft Graph prostřednictvím vaší aplikace, zpochybněn kvůli dalším informacím, které nejsou v přístupovém tokenu, který vaše aplikace původně získala. V takovém případě se při akvizici přístupového tokenu zobrazí chyba 400 se zprávou *interaction_required* nebo se při volání Microsoft Graphu zobrazí chyba403 se zprávou *insufficient_claims*. V obou případech obsahuje odpověď na chybu další informace, které lze prezentovat autorizačnímu koncovému bodu a vyzvat uživatele k dalším informacím (jako je vícefaktorové ověřování nebo registrace zařízení).

- [Řešení problémů s podmíněným přístupem pomocí funkce MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Pokyny pro vývojáře k podmíněnému přístupu k Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
