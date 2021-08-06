---
title: Dotazování na rozhraní Microsoft Graph API
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923232"
---
# <a name="querying-the-microsoft-graph-api"></a>Dotazování na rozhraní Microsoft Graph API

Toto téma se může taky vztahovat na vývojáře, kteří stále používají rozhraní Api Graph Azure AD. Důrazně se ale **doporučuje používat** Microsoft Graph pro všechny scénáře správy adresáře, identity a přístupu.

**Problémy s ověřováním nebo autorizací**

- Pokud vaše aplikace nemůže získat **tokeny** pro volání do Microsoft Graph, vyberte Problém s získáním kategorie **přístupového tokenu (Ověřování)** Microsoft Graph, abyste získali konkrétnější nápovědu a podporu k tomuto tématu.
- Pokud se v aplikaci při volání microsoftu Graph zobrazí chyby autorizace **401 nebo 403,** vyberte kategorii Získání chyby odepření přístupu **(Autorizace)** rozhraní Microsoft Graph API a získejte konkrétnější nápovědu a podporu k tomuto tématu.

**Chci používat Microsoft Graph, ale nejste si jistí, kde začít**

Další informace o microsoftové Graph najdete v tématu:

- [Přehled microsoftových Graph](https://docs.microsoft.com/graph/overview)
- [Přehled správy identit a přístupu v Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začínáme s vytvářením aplikací Microsoft Graph aplikací](https://docs.microsoft.com/graph/)
- **Průzkumník Graph Microsoftu** – testování rozhraní API Graph Microsoftu ve vašem tenantovi nebo ukázkovém tenantovi

**Chci používat Microsoft Graph, ale podporuje rozhraní API adresáře v1.0, která potřebuji?**

Microsoft Graph je doporučené rozhraní API pro správu adresářů, identit a přístupu. Mezi tím, co je možné v Azure AD Graph a Microsoft Graph, je ale stále několik mezer. Projděte si následující články, které zvýrazňují nejnovější rozdíly, které vám pomohou při výběru:

- [Rozdíly typu prostředků mezi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdíly vlastností mezi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdíly mezi metodami Azure AD a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Při dotazu na *objekt uživatele* chybí mnoho jeho vlastností.**

`GET https://graph.microsoft.com/v1.0/users`Vrátí jenom 11 vlastností, protože Graph automaticky vybere výchozí  sadu uživatelských vlastností, které se mají vrátit. Pokud potřebujete další *uživatelské vlastnosti,* $select vyberte vlastnosti, které aplikace potřebuje. Vyzkoušejte si to nejdřív **v Microsoft Graph Exploreru.**

**Některé hodnoty vlastností uživatele mají *hodnotu Null,* i když vím, že jsou nastavené.**

Nejpravděpodobnější vysvětlení je, že aplikaci bylo uděleno *oprávnění User.ReadBasic.All.* Aplikace tak může číst omezenou sadu vlastností uživatele a vrátit všechny ostatní vlastnosti jako null, i když byly dříve nastavené. Zkuste místo toho udělit *aplikaci User.Read.All* oprávnění.

Další informace najdete v tématu [Microsoft Graph oprávnění uživatelů](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Mám potíže s použitím parametrů dotazu OData k filtrování dat v mých žádostech.**

Microsoft Graph sice podporuje širokou škálu parametrů dotazu OData, ale mnoho z těchto parametrů není plně podporováno adresářovou službou (prostředky, které dědí z *objektu directoryObject)* v Microsoft Graph. Stejná omezení, která byla ve službě Azure AD Graph v Microsoftu ve většině Graph:

1. **Není podporováno:**$count, $search a $filter hodnoty *null* nebo *ne*
2. **Není podporováno:**$filter určitých vlastnostech (viz témata zdrojů, u kterých jsou vlastnosti filtrovatelné)
3. **Nepodporuje se**: stránkování, filtrování a řazení najednou
4. **Nepodporuje se**: filtrování relace. Například – najděte všechny členy technické skupiny, které jsou ve Velké Británii.
5. **Částečná podpora:**$orderby *uživatele* (pouze displayName a userPrincipalName) a *skupina*
6. Částečná **podpora:**$filter (podporuje jenom *eq*,  *startswith* nebo *,* a a omezená ) podpora, $expand (rozšíření relací jednoho objektu vrátí všechny relace, ale rozšíření kolekce relací objektů je omezené)

Další informace najdete v tématu [Přizpůsobení odpovědí pomocí parametrů dotazu](https://docs.microsoft.com/graph/query-parameters).

**Rozhraní API, které volám, nefunguje – kde můžu dělat další testování?**

**Průzkumník Graph Microsoftu** – otestujte rozhraní MICROSOFT Graph API ve vašem tenantovi  nebo ukázkovém tenantovi a podívejte se také na ukázkové dotazy v Průzkumníku Microsoft Graph Exploreru.

**Když se dotazuji na data, zdá se, že se mi vrací neúplná sada dat.**

Pokud se dotazuje na kolekci (třeba *uživatelé),* microsoft Graph používá limity stránek na straně serveru, takže výsledky se vždycky vrátí s výchozí velikostí stránky. Vaše aplikace by měla vždy očekávat, že bude procházet kolekcemi vrácených ze služby.

Další informace najdete tady:

- [Doporučené Graph microsoftu](https://docs.microsoft.com/graph/best-practices-concept)
- [Stránkování microsoftových Graph ve vaší aplikaci](https://docs.microsoft.com/graph/paging)

**Moje aplikace je příliš pomalá a taky se ztuhá. Jaká vylepšení můžu udělat?**

V závislosti na vašem scénáři máte k dispozici různé možnosti, jak zajistit, aby vaše aplikace byla výkonnější, a v některých případech méně náchylná k omezení službou (když provádíte příliš mnoho hovorů).

Více k tomu najdete tady:

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
