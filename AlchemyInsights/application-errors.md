---
title: Chyby aplikací
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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984517"
---
# <a name="application-errors"></a>Chyby aplikací

Hledáte informace o **kódech chyb AADSTS** , které se vracejí ze služby tokenů zabezpečení Azure Active Directory (STS)? Čtením [kódů chyb ověřování a autorizace Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) najdete AADSTS Popis chyb, opravy a některá navrhovaná řešení.

Chyby autorizace můžou být výsledkem několika různých problémů, z nichž většinu generuje chybu 401 nebo 403. V následujícím příkladu mohou všechny vést k chybám autorizace:

- Nesprávné [toky získání přístupových tokenů](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Špatně nakonfigurované [obory oprávnění](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Nedostatek [souhlasu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Pokud chcete vyřešit běžné chyby autorizace, vyzkoušejte následující kroky, které se nejvíce shodují s chybou, kterou jste dostali. Můžete použít více než jednu.

**401 neoprávněná Chyba: je váš token platný?**

Ujistěte se, že aplikace v rámci žádosti prezentuje v aplikaci Microsoft Graph platný přístupový token. Tato chyba často znamená, že přístupový token možná v záhlaví žádosti HTTP Authenticate chybí nebo že je neplatný nebo vypršela jeho platnost. Důrazně doporučujeme, abyste pro získání accessového tokenu použili [knihovnu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) . K této chybě může navíc dojít, pokud se pokusíte použít delegovaný přístupový token udělený osobnímu účtu Microsoft pro přístup k rozhraní API, které podporuje jenom pracovní nebo školní účty (organizační účty).

**403, chyba: zvolili jste správnou sadu oprávnění?**

Zkontrolujte, jestli jste požadovali správnou sadu oprávnění založenou na rozhraních API Microsoft graphu pro hovory. Doporučená nejméně privilegovaná oprávnění jsou k dispozici ve všech tématech referenční metody rozhraní Microsoft Graph API. Kromě toho musí být tato oprávnění přidělena uživateli nebo správcem. K udělení oprávnění obvykle dochází prostřednictvím stránky souhlasu nebo udělením oprávnění pomocí registračního panelu aplikace Azure Portal. V okně **Nastavení** aplikace klikněte na **požadovaná oprávnění** a potom na **udělit oprávnění**.

- [Oprávnění pro Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Principy oprávnění a souhlasu služby Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 zakázaná Chyba: aplikace získala token pro přiřazení zvolených oprávnění?**

Ujistěte se, že typ požadovaného nebo přiděleného oprávnění odpovídá typu přístupového tokenu, který aplikace získává. Je možné, že budete požádáni o oprávnění a udělujete oprávnění k aplikacím, ale místo tokenů toku přihlašovacích údajů klienta nebo při požadování a udělování delegovaných oprávnění, ale pomocí tokenů toku kódu, ale s využitím tokenů toku kódu.

- [Získání přístupu pro uživatele a delegovaná oprávnění](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0 – tok autorizačního kódu OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získání přístupu bez uživatele (služby démon) a oprávnění aplikace](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0 – tok přihlašovacích údajů klienta OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403, chyba: resetování hesla**

Aktuálně nejsou k dispozici žádná oprávnění služby typu démon oprávnění aplikace, která povolují Resetování uživatelských hesel. Tato rozhraní API jsou podporovaná jenom pomocí interaktivního toku kódu delegovaného pomocí přihlášeného správce.

- [Oprávnění pro Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 zakázáno: uživatel má přístup a mají licenci?**

V případě toků delegovaných kódů Microsoft Graph vyhodnotí, jestli je žádost povolená na základě oprávnění udělených aplikaci a oprávnění, která má přihlášený uživatel. Tato chyba obecně znamená, že uživatel nemá dostatečná oprávnění k provádění žádosti nebo jestli uživatel nemá licenci na data, ke kterým přistupuje. Žádost se můžou úspěšně uskutečnit jenom uživatelé s požadovanými oprávněními nebo licencemi.

**403 zakázáno: vybrali jste správné rozhraní API prostředku?**

Služby API (jako je Microsoft Graph): Zkontrolujte, že AUD deklarace (cílová skupina) v přijatém přístupovém tokenu odpovídá hodnotě, kterou očekává pro sebe, a pokud ne, bude výsledkem Chyba 403 Forbidden. Běžná chyba, která je výsledkem této chyby, se pokouší použít token získaný pro rozhraní API Azure AD, rozhraní API aplikace Outlook nebo rozhraní API SharePointu nebo OneDrivu pro volání do Microsoft graphu (nebo naopak). Ujistěte se, že prostředek (nebo obor) aplikace získává token pro odpovídající rozhraní API, na které aplikace volá.

**400 nesprávný požadavek nebo 403 zakázáno: uživatel dodržuje zásady pro podmíněné přístup k organizaci (CÚ)?**

Na základě zásad certifikačního úřadu organizace může být uživatel, který přistupuje k prostředkům Microsoft graphu prostřednictvím aplikace, požádán o další informace, které se nenacházejí v přístupovém tokenu, který aplikace původně získala. V tomto případě vám aplikace obdrží 400 s chybou *interaction_required* během získávání accessového tokenu nebo 403 s chybou *insufficient_claims* při volání do Microsoft graphu. V obou případech odpověď na chybu obsahuje další informace, které se dají uživateli dát k dispozici koncovému bodu autorizace, aby mohl uživatele pověřit další informace (jako je třeba vícefaktorové ověřování nebo registrace zařízení).

- [Zpracování výzev k podmíněnému přístupu pomocí MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Návod pro vývojáře pro podmíněný přístup k Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
