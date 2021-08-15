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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975886"
---
# <a name="microsoft-graph-api-issues"></a>Problémy s rozhraním Microsoft Graph API

Toto téma se může taky vztahovat na vývojáře, kteří stále používají rozhraní Api Graph Azure AD. Důrazně se ale **doporučuje používat** Microsoft Graph pro všechny scénáře správy adresáře, identity a přístupu.

**Problémy s ověřováním nebo autorizací**

- Pokud vaše aplikace nemůže získat **tokeny** pro volání do Microsoft Graph, vyberte Problém s získáním kategorie **přístupového tokenu (Ověřování)** Microsoft Graph, abyste získali konkrétnější nápovědu a podporu k tomuto tématu.
- Pokud se v aplikaci při volání microsoftu Graph zobrazí chyby autorizace **401 nebo 403,** vyberte kategorii Získání chyby odepření přístupu **(Autorizace)** rozhraní Microsoft Graph API a získejte konkrétnější nápovědu a podporu k tomuto tématu.

**Chci používat Microsoft Graph, ale nejste si jistí, kde začít**

- [Přehled microsoftových Graph](https://docs.microsoft.com/graph/overview)
- [Přehled správy identit a přístupu v Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začínáme s vytvářením aplikací Microsoft Graph aplikací](https://docs.microsoft.com/graph/)
- **Průzkumník Graph Microsoftu** – testování rozhraní API Graph Microsoftu ve vašem tenantovi nebo ukázkovém tenantovi

**Chci používat Microsoft Graph, ale podporuje rozhraní API adresáře v1.0, která potřebuji?**

Microsoft Graph je doporučené rozhraní API pro správu adresářů, identit a přístupu. Mezi tím, co je možné v Azure AD Graph a Microsoft Graph, je ale stále několik mezer. Projděte si následující články, které zvýrazňují nejnovější rozdíly, které vám pomohou při výběru:

- [Rozdíly typu prostředků mezi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdíly vlastností mezi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdíly mezi metodami Azure AD a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Rozhraní API, které volám, nefunguje – kde můžu dělat další testování?**

**Průzkumník Graph Microsoftu** – otestujte rozhraní MICROSOFT Graph API ve vašem tenantovi  nebo ukázkovém tenantovi a podívejte se také na ukázkové dotazy v Průzkumníku Microsoft Graph Exploreru.

**Moje aplikace je příliš pomalá a taky se ztuhá. Jaká vylepšení můžu udělat?**

V závislosti na vašem scénáři máte k dispozici celou řadu možností, jak zajistit, aby vaše aplikace byla výkonnější a v některých případech méně náchylná k omezení službou (když provádíte příliš mnoho hovorů).

- [Doporučené Graph microsoftu](https://docs.microsoft.com/graph/best-practices-concept)
- [Žádosti o dávku](https://docs.microsoft.com/graph/json-batching)
- [Sledování změn pomocí rozdílového dotazu](https://docs.microsoft.com/graph/delta-query-overview)
- [Oznámení o změnách prostřednictvím webhooků](https://docs.microsoft.com/graph/webhooks)
- [Pokyny k omezení](https://docs.microsoft.com/graph/throttling)

**Kde najdu další informace o chybách a známých problémech?**

- [Informace o Graph chyb microsoftu](https://docs.microsoft.com/graph/errors)
- [Známé problémy s Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kde můžu zkontrolovat stav dostupnosti služby a připojení?**

Dostupnost služeb a připojení podkladových služeb, ke kterým je možné přistupovat prostřednictvím Microsoft Graph, může mít vliv na celkovou dostupnost a výkon microsoftových Graph.

- Pokud Azure Active Directory stavu služby, zkontrolujte stav **služeb Zabezpečení a identit** uvedených na stránce stavu [Azure](https://azure.microsoft.com/status/).
- Pokud Office služby, které přispívají k microsoftu Graph, zkontrolujte stav služeb uvedených v [řídicím](https://portal.office.com/adminportal/home#/servicehealth)panelu Office stavu služby .

Chyby Graph může být výsledkem několika různých problémů, z nichž většina generuje chybu 401 nebo 403. K chybám autorizace může například vést následující:

- Nesprávné [toky akvizice přístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Špatně nakonfigurované [rozsahy oprávnění](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Chybějící [souhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Ukončení podpory knihovny Azure Active Directory ověřování (ADAL) a rozhraní API služby Azure AD Graph (AAD Graph)***

**Od 30. června 2020** už nebudeme přidávat žádné nové funkce do ADAL a Azure AD Graph. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.

**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a už nebudeme poskytovat technickou podporu ani aktualizace zabezpečení.

Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po této době fungovat, ale nebudou dostávat technickou podporu ani *aktualizace zabezpečení*.

Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graph azure ad.

**Migrace ADAL**

Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.

Pokud používáte aplikace Microsoft, víte, že Microsoft do konečného termínu ukončení podpory migruje své aplikace na MSAL, což zajistí, že budou mít prospěch z průběžného zabezpečení a vylepšení funkcí společnosti MSAL.

1. [Přečtěte si časté otázky k ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informace o tom, jak migrovat aplikace na základě platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Pokud potřebujete pomoc s pochopením, které z vašich aplikací používají ADAL, doporučujeme zkontrolovat zdrojový kód všech aplikací a případně kontaktovat poskytovatele internetových služeb nebo poskytovatelů aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají Azure AD Graph, postupujte podle našich pokynů k migraci [aplikací Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)na Microsoft Graph .

1. [Základní informace najdete v našem kontrolním seznamu migrace](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací. Podpora Microsoftu vám taky může poskytnout seznam všech využití služby AAD Graph ve vašem tenantovi.
3. Aby vaše aplikace přistupovat k datům v microsoft Graph, musí mu uživatel nebo správce udělit správná oprávnění prostřednictvím procesu souhlasu. Odkaz [microsoft Graph oprávnění](https://docs.microsoft.com/graph/permissions-reference) uvádí oprávnění přidružená ke každé hlavní sadě rozhraní Microsoft Graph API. Obsahuje také pokyny k používání oprávnění.
