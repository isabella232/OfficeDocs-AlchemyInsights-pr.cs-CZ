---
title: Problémy s rozhraním Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713470"
---
# <a name="microsoft-graph-api-issues"></a>Problémy s rozhraním Microsoft Graph API

Toto téma se může také vztahovat na vývojáře, kteří stále používají rozhraní Azure AD Graph API. Důrazně ale **doporučujeme** používat Microsoft Graph pro všechny scénáře správy adresářů, identit a přístupu.

**Problémy s ověřováním nebo autorizacem**

- Pokud aplikace nemůže získat **tokeny,** které volají na Microsoft Graph, vyberte Problém se získáním kategorie Microsoft **Graphu pro přístupový token (ověřování),** abyste získali konkrétnější nápovědu a podporu pro toto téma.
- Pokud aplikace dostává při volání Microsoft Graphu chyby autorizace **401 nebo 403,** vyberte kategorii Získání chyby odepření přístupu **(autorizace)** rozhraní Microsoft Graph API, abyste získali konkrétnější nápovědu a podporu k tomuto tématu.

**Chci používat Microsoft Graph, ale nevím, kde začít**

- [Základní informace o Microsoft Graphu](https://docs.microsoft.com/graph/overview)
- [Přehled správy identit a přístupu v aplikaci Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začínáme s vytvářením aplikací Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Testování rozhraní Microsoft Graph API ve vašem tenantovi nebo ukázkovém tenantovi

**Chci používat Microsoft Graph, ale podporuje rozhraní API adresáře v1.0, která potřebuji?**

Microsoft Graph je doporučené rozhraní API pro správu adresáře, identity a přístupu. Mezi tím, co je možné v Azure AD Graphu a Microsoft Graphu, je ale pořád pár mezer. Projděte si následující články, ve kterých jsou uvedené nejnovější rozdíly, které vám pomohou při výběru:

- [Rozdíly typů zdrojů mezi Azure AD Graph a Microsoft Graphem](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdíly ve vlastnostech mezi Azure AD Graph a Microsoft Graphem](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdíly mezi metodami mezi Azure AD a Microsoft Graphem](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Rozhraní API, které volám, nefunguje – kde můžu dělat další testování?**

**Microsoft Graph Explorer** – Otestujte rozhraní Microsoft Graph API ve vašem tenantovi nebo ukázkovém tenantovi a také se podívejte na ukázkové dotazy **v** Microsoft Graph Exploreru.

**Moje aplikace je příliš pomalá a zároveň se zhroucela. Jaká vylepšení můžu udělat?**

V závislosti na vašem scénáři se k dispozici různé možnosti, jak zajistit výkon aplikace, a v některých případech je méně náchylná k omezení služby (když provádíte příliš mnoho hovorů).

- [Doporučené postupy pro Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Žádosti o dávku](https://docs.microsoft.com/graph/json-batching)
- [Sledování změn prostřednictvím rozdílového dotazu](https://docs.microsoft.com/graph/delta-query-overview)
- [Oznámení o změnách prostřednictvím webhooků](https://docs.microsoft.com/graph/webhooks)
- [Pokyny pro omezení](https://docs.microsoft.com/graph/throttling)

**Kde najdu další informace o chybách a známých problémech?**

- [Informace o odpovědi na chyby v Microsoft Graphu](https://docs.microsoft.com/graph/errors)
- [Známé problémy s Microsoft Graphem](https://docs.microsoft.com/graph/known-issues)

**Kde můžu zkontrolovat stav dostupnosti a připojení služeb?**

Dostupnost služeb a připojení základních služeb, ke kterým se můžete dostat přes Microsoft Graph, může mít vliv na celkovou dostupnost a výkon Microsoft Graphu.

- Pokud chcete zjistit stav služby Azure Active Directory, zkontrolujte stav služeb **Security + Identity,** které jsou uvedené na [stránce stavu Azure.](https://azure.microsoft.com/status/)
- U služeb Office, které do Microsoft Graphu přispívají, se podívejte na stav služeb uvedených na řídicím panelu [stavu služeb Office.](https://portal.office.com/adminportal/home#/servicehealth)

Chyby autorizace Aplikace Microsoft Graph mohou být výsledkem několika různých problémů, z nichž většina vygeneruje chybu 401 nebo 403. Například následující příklad může vést k chybám autorizace:

- Nesprávné [toky akvizice přístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Špatně nakonfigurované [rozsahy oprávnění](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Chybějící [souhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Konec podpory pro knihovnu Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD Graph (AAD Graph)_* _

_*Od 30. června 2020** nebudeme do ADAL a Azure AD Graph přidávat žádné nové funkce. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.

**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a nebudeme už poskytovat technickou podporu ani aktualizace zabezpečení.

Aplikace používající ADAL ve stávajících verzích operačního systému budou i po této době dál fungovat, ale nebudou dostávat žádné aktualizace technické podpory ani *zabezpečení.*

Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graphu.

**Migrace ADAL**

Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.

Pokud používáte aplikace Microsoftu, věděli jste, že Microsoft do konečného termínu ukončení podpory migruje aplikace na msal, a zajišťuje tak, že pro msAL budou využívat průběžná vylepšení zabezpečení a funkcí.

1. [Přečtěte si časté otázky k ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informace o tom, jak migrovat aplikace na základě platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Pokud potřebujete pomoct s pochopením, která z vašich aplikací používá ADAL, doporučujeme zkontrolovat si zdrojový kód všech aplikací, a pokud je to možné, kontaktovat některé isVs nebo poskytovatele aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají Azure AD Graph, postupujte podle pokynů k migraci aplikací [Azure AD Graph do Microsoft Graphu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Základní informace najdete v našem kontrolním seznamu migrace](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací. Podpora Microsoftu vám také může poskytnout seznam všech využití AAD Graphu ve vašem tenantovi.
3. Aby vaše aplikace získá přístup k datům v Microsoft Graphu, musí ji uživatel nebo správce udělit správná oprávnění prostřednictvím procesu udělení souhlasu. Odkaz [na oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference) obsahuje oprávnění přidružená k jednotlivým hlavním sadě rozhraní Microsoft Graph API. Obsahuje taky pokyny, jak tato oprávnění používat.
