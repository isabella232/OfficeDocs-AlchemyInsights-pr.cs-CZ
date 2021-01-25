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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974233"
---
# <a name="authentication-issues"></a>Problémy s ověřováním

**Hledáte informace o kódech chyb AADSTS, které jsou vraceny ze služby tokenů zabezpečení Azure Active Directory (STS)?** Pokud chcete najít AADSTS Popis chyb, opravy a některá navrhovaná řešení, podívejte se na [kódy chyb ověřování a autorizace Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) .

Chyby autorizace můžou být výsledkem několika různých problémů, z nichž většinu generuje chybu 401 nebo 403. Všechny následující problémy mohou vést k chybám autorizace:

- Nesprávné [toky získání přístupových tokenů](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Špatně nakonfigurované [obory oprávnění](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Nedostatek [souhlasu](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Pokud chcete vyřešit běžné chyby autorizace, vyzkoušejte následující kroky, které se nejvíce shodují s chybou, kterou jste dostali. Pro chybu, kterou přijímáte, se může vztahovat více kroků.

- **401 neoprávněná Chyba: je váš token platný?**

Ujistěte se, že aplikace prezentuje jako součást žádosti platný přístupový token do Microsoft graphu. Tato chyba často znamená, že přístupový token možná v záhlaví žádosti HTTP Authenticate chybí nebo že je neplatný nebo vypršela jeho platnost. Důrazně doporučujeme, abyste pro získání accessového tokenu použili knihovnu Microsoft Authentication Library (MSAL). K této chybě může navíc dojít, pokud se pokusíte použít delegovaný přístupový token udělený osobnímu účtu Microsoft pro přístup k rozhraní API, které podporuje jenom pracovní nebo školní účty (organizační účty).

**403, chyba: zvolili jste správnou sadu oprávnění?**

Ujistěte se, že jste požadovali správnou sadu oprávnění založenou na rozhraních API Microsoft graphu pro hovory. Doporučená oprávnění s nejnižším oprávněním jsou k dispozici ve všech tématech referenční metody rozhraní Microsoft Graph API. Kromě toho musí být tato oprávnění přidělena uživateli nebo správcem. K udělení oprávnění obvykle dochází prostřednictvím stránky souhlasu nebo pomocí registračního panelu aplikace Azure Portal. V okně **Nastavení** aplikace klikněte na **požadovaná oprávnění** a potom na **udělit oprávnění**. Další informace najdete tady:

- [Oprávnění pro Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Principy oprávnění a souhlasu služby Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 zakázaná Chyba: aplikace získala token pro přiřazení zvolených oprávnění?**

Zajistěte, aby typy požadovaných oprávnění odpovídaly typu přístupového tokenu, který aplikace získává. Je možné, že budete požádáni o oprávnění aplikací a místo tokenů toku přihlašovacích údajů klienta, ale s použitím tokenů toku přihlašovacích údajů klienta namísto delegovaných tokenů toku kódu.

Další informace o získání tokenů najdete v tématech:

- [Získání přístupu pro uživatele a delegovaná oprávnění](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0 – tok autorizačního kódu OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získání přístupu bez uživatele (služby démon) a oprávnění aplikace](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0 – tok přihlašovacích údajů klienta OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403, chyba: resetování hesla**

Aktuálně nejsou k dispozici žádná oprávnění služby typu démon oprávnění aplikace, která povolují Resetování uživatelských hesel. Tato rozhraní API jsou podporovaná jenom pomocí interaktivního toku kódu delegovaného pomocí přihlášeného správce. Další informace najdete v tématu [oprávnění aplikace Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 zakázáno: uživatel má přístup a mají licenci?**

V případě toků delegovaných kódů Microsoft Graph vyhodnocuje, jestli je žádost povolená na základě oprávnění udělených aplikaci a oprávnění, která má přihlášený uživatel. Tato chyba obecně znamená, že uživatel nemá dostatečná oprávnění k provádění žádosti **nebo** jestli uživatel nemá licenci na data, ke kterým přistupuje. Žádost se můžou úspěšně uskutečnit jenom uživatelé s požadovanými oprávněními nebo licencemi.

**403 zakázáno: vybrali jste správné rozhraní API prostředku?**

Služby API, jako je Microsoft Graph: Zkontrolujte, že *AUD* deklarace (cílová skupina) v přijatém přístupovém tokenu odpovídá hodnotě, kterou očekává, a pokud ne, dojde k chybě v 403. Běžná chyba, která je výsledkem této chyby, se pokouší použít token získaný pro rozhraní API Azure AD, rozhraní API aplikace Outlook nebo rozhraní API SharePointu nebo OneDrivu pro volání do Microsoft graphu (nebo naopak). Ujistěte se, že prostředek (nebo obor) aplikace získává token pro odpovídající rozhraní API, na které aplikace volá.

**400 nesprávný požadavek nebo 403 zakázáno: uživatel dodržuje zásady pro podmíněné přístup k organizaci (CÚ)?**

Na základě zásad podmíněného přístupu pro organizace (CÚ) se může stát, že uživatel, který přistupuje k prostředkům Microsoft graphu prostřednictvím aplikace, bude požádán o další informace, které se nenacházejí v přístupovém tokenu, který jste původně získali. V tomto případě vám aplikace obdrží **400 s chybou *interaction_required*** během získávání accessového tokenu nebo **403 s chybou *insufficient_claims*** při volání do Microsoft graphu. V obou případech odpověď na chybu obsahuje další informace, které mohou být prezentovány koncovému bodu k tomu, aby mohl uživatele dát k dispozici další informace (například vícefaktorové ověřování nebo zápis zařízení).

Další informace o podmíněném přístupu najdete v těchto tématech:

- [Zpracování výzev k podmíněnému přístupu pomocí MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Návod pro vývojáře pro podmíněný přístup k Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Konec podpory knihovny služby Azure Active Directory (ADAL) a rozhraní API služby Azure AD Graph (graf AAD)_* _

- Po zahájení června 2020 nepřidáme do knihovny Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD graphu žádné nové funkce. Budeme dál poskytovat technické podpory a aktualizace zabezpečení, ale nebudete už poskytovat aktualizace funkcí.
- Od června 2022, my vám ukončí podporu pro graf ADAL a AAD a nebude už poskytovat technickou podporu ani aktualizace zabezpečení.
    - Aplikace používající ADAL v existujících verzích OS budou po této době dál fungovat, ale nezískají žádné technické podpory ani aktualizace zabezpečení.
    - Aplikace používající v grafu AAD po této době nemusí dostávat odpovědi z koncového bodu grafu AAD.

_ *Migrace**

Doporučujeme aktualizovat [knihovnu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení. Toto doporučení je v kontextu Microsoft, který migruje své aplikace tak, aby MSAL od konečného termínu podpory. Cílem migrace aplikací Microsoftu na MSAL je zajistit, aby aplikace využily výhod vylepšeného zabezpečení a funkcí MSAL.

- [Přečtěte si část časté otázky](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informace o migraci aplikací na základě jednotlivých platforem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Pokud potřebujete pomoct s porozuměním, které z vašich aplikací používá ADAL, doporučujeme, abyste si provedli kontrolu všech nezávislých dodavatelů softwaru (ISV) nebo poskytovatelů aplikací, a pokud se to týká. Podpora Microsoftu vám taky poskytne seznam všech aplikací ADAL, které nejsou od Microsoftu, ve vašem tenantovi.

**Migrace grafu AAD**

U aplikací, které používají graf AAD, postupujte podle pokynů pro [migraci aplikací Graph AD služby graf v Azure do Microsoft graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Naše kontrolní seznam migrace představuje bod Začínáme](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portál registrace aplikací pro Azure zobrazuje, které aplikace používají graf AAD. Doporučujeme, abyste zkontrolovali všechny zdrojové kódy aplikací a pokud jsou k dispozici, a pokud je to možné, kontaktujte všechny poskytovatele ISV nebo aplikace. Podpora Microsoftu vám taky poskytne informace o všech použitích grafu AAD ve vašem tenantovi.

 










