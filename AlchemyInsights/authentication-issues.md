---
title: Problémy s ověřováním
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019501"
---
# <a name="authentication-issues"></a>Problémy s ověřováním

**Hledáte informace o kódech chyb AADSTS vrácených ze služby tokenů zabezpečení Azure Active Directory (Azure AD)?** V tématu [Kódy chyb ověřování Azure AD a autorizace](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) najdete popisy chyb AADSTS, opravy a některá navrhovaná řešení.

Chyby autorizace mohou být výsledkem několika různých problémů, z nichž většina vygeneruje chybu 401 nebo 403. K chybám autorizace mohou vést například následující problémy:

- Nesprávné [toky akvizice přístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Špatně nakonfigurované [rozsahy oprávnění](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Chybějící [souhlas](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Pokud chcete vyřešit běžné chyby autorizace, vyzkoušejte níže uvedené kroky, které co nejvíce odpovídají zobrazené chybě. Chybě, která s vám zobrazuje, může odpovídat více než jeden krok.

**401 Unauthorized error: Is your token valid?** (401 Chyba autorizace: Máte platný token?)

Ujistěte se, že aplikace v rámci žádosti předkládá Microsoft Graphu platný přístupový token. Tato chyba často znamená, že v záhlaví žádosti o ověření protokolu HTTP chybí přístupový token, že je token neplatný nebo že vypršela jeho platnost. Důrazně doporučujeme používat pro získání přístupových tokenů knihovnu Microsoft Authentication Library (MSAL). K této chybě může navíc dojít, když se pokusíte použít delegovaný přístupový token udělený osobnímu účtu Microsoft pro přístup k rozhraní API, které podporuje jenom pracovní nebo školní účty (účty organizace).

**403 Forbidden error: Have you chosen the right set of permissions?** (chyba 403 Zakázáno: Vybrali jste správnou sadu oprávnění?)

Ujistěte se, že jste poslali požadavek na správnou sadu oprávnění podle rozhraní API Microsoft Graph, které vaše aplikace volá. Doporučená nejméně privilegovaná oprávnění jsou k dispozici ve všech tématech o referenčních metodách rozhraní API Microsoft Graphu. Tato oprávnění musí navíc aplikaci udělit uživatel nebo správce. Oprávnění se obvykle uděluje na stránce souhlasu nebo použitím okna registrace aplikace na portálu Azure Portal. V okně **Nastavení** aplikace klikněte na **Povinná oprávnění** a potom na **Udělit oprávnění**. Další informace najdete tady:

- [Oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference) 
- [Principy oprávnění a souhlasu v Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Forbidden error: Did your app acquire a token to match chosen permissions?** (chyba 403 Zakázáno: Získala vaše aplikace token odpovídající vybraným oprávněním?)

Ujistěte se, že se požadované nebo udělené typy oprávnění shodují s typem přístupového tokenu, který aplikace získá. Možná při podávání žádostí a udělování oprávnění aplikacím používáte tokeny pro delegované interaktivní toky kódu místo tokenů pro tok přihlašovacích údajů klienta, nebo při podávání žádostí a udělování delegovaných oprávnění používáte tokeny pro tok přihlašovacích údajů klienta místo tokenů pro delegované interaktivní toky kódu.

Další informace o získávání tokenů najdete v těchto tématech:

- [Získání přístupu jménem uživatelů a delegovaná oprávnění](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – tok autorizačního kódu OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získání přístupu bez oprávnění pro uživatele (služba proces démona) a aplikace](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – tok přihlašovacích údajů klienta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Forbidden error: Resetting password** (chyba 403 Zakázáno: Resetování hesla)

V současné době neexistují žádná oprávnění typu služba-služba pro oprávnění aplikací procesu démona, která by umožnila resetování uživatelských hesel. Tato rozhraní API jsou podporovaná jenom přes delegované interaktivní toky kódu s přihlášeným správcem. Další informace najdete v tématu [Oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference).

**403 Forbidden: Does the user have access and are they licensed?** (403 Zakázáno: Má uživatel přístup a licenci?)

U delegovaných toků kódu vyhodnotí Microsoft Graph informaci, jestli je žádost povolená, na základě oprávnění udělených aplikaci a oprávnění, která má přihlášený uživatel. Tato chyba obecně znamená, že uživatel nemá dostatečná oprávnění k provedení žádosti **nebo** nemá licenci pro přístup k požadovaným datům. Žádost můžou úspěšně provést jenom uživatelé s požadovanými oprávněními nebo licencemi.

**403 Forbidden: Did you select the correct resource API?** (403 Zakázáno: Vybrali jste správné rozhraní API prostředku?)

Služby API, jako je Microsoft Graph, kontrolují, jestli nárok *aud* (cílová skupina) v přijatém přístupového tokenu odpovídá hodnotě, kterou pro sebe očekává, a pokud ne, dojde k chybě 403 Zakázáno. Běžný omyl, který vede k této chybě, je použití tokenu získaného pro rozhraní API Azure AD Graphu, rozhraní API Outlooku nebo rozhraní API SharePointu/OneDrivu k volání Microsoft Graphu (nebo naopak). Ujistěte se, že prostředek (nebo obor), pro který vaše aplikace získává token, odpovídá rozhraní API, které aplikace volá.

**400 Bad Request / 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?** (400 Nesprávná žádost / 403 Zakázáno: Splňuje uživatel zásady podmíněného přístupu organizace (CA)?)

Na základě zásad podmíněného přístupu organizace (CA) můžou být od uživatele přistupujícího k prostředkům Microsoft Graphu prostřednictvím vaší aplikace vyžadovány další informace, které nejsou v přístupovém tokenu původně získaném vaší aplikací. V takovém případě se při akvizici přístupového tokenu zobrazí chyba **400 se zprávou *interaction_required*** nebo se při volání Microsoft Graphu zobrazí chyba **403 se zprávou *insufficient_claims***. V obou případech obsahuje odpověď na chybu další informace, které je možné předložit autorizovanému koncovému bodu a vyzvat tak uživatele k zadání dalších informací (například pomocí vícefaktorového ověřování nebo registrace zařízení).

Další informace o podmíněném přístupu najdete v těchto tématech:

- [Řešení problémů s podmíněným přístupem pomocí MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Pokyny pro vývojáře k podmíněnému přístupu k Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Ukončení podpory knihovny Azure Active Directory ověřování (ADAL) a rozhraní API služby Azure AD Graph (AAD Graph)***

- Od 30. června 2020 už nebudeme do knihovny Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD Graph (AAD Graph) přidávat žádné nové funkce. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.
- Od 30. června 2022 ukončíme podporu pro ADAL a AAD Graph a nebudeme už poskytovat technickou podporu ani aktualizace zabezpečení.
    - Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po tomto datu fungovat, ale nebudou mít technickou podporu ani aktualizace zabezpečení.
    - Aplikace používající AAD Graph už po tomto datu nebudou přijímat odpovědi z koncového bodu AAD Graphu.

**Migrace ADAL**

Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení. Toto doporučení je platné v kontextu migrace aplikací Microsoftu do knihovny MSAL v rámci konečného termínu ukončení podpory. Cílem migrace aplikací Microsoftu do knihovny MSAL je zajištění výhod průběžných vylepšení zabezpečení a funkcí v knihovně MSAL.

- [Přečtěte si časté otázky k ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informace o tom, jak migrovat aplikace na základě platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Pokud potřebujete pomoct zjistit, které z vašich aplikací používají ADAL, doporučujeme zkontrolovat zdrojový kód všech vašich aplikací, a pokud to bude možné, kontaktovat nezávislé dodavatele softwaru (ISV) nebo poskytovatele aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají AAD Graph, postupujte podle pokynů k [migraci aplikací Azure AD Graph do Microsoft Graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Základní informace najdete v našem kontrolním seznamu migrace](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací. Informace o veškerém využití AAD Graphu na vašem tenantovi vám může poskytnout taky podpora Microsoftu.

 










