---
title: Dotazování rozhraní Microsoft Graph API
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974216"
---
# <a name="querying-the-microsoft-graph-api"></a>Dotazování rozhraní Microsoft Graph API

Toto téma se taky bude vztahovat na vývojáře, kteří ještě používají API Azure AD Graph. Ve scénářích pro správu adresářů, identit a Access se ale **důrazně** doporučuje používat Microsoft Graph.

**Problémy s ověřováním nebo autorizací**

- Pokud se vaší aplikací **nepodaří získat tokeny** pro volání do aplikace Microsoft Graph, vyberte **problém se získáním přístupového tokenu (Authentication)** kategorie Microsoft graphu a získejte konkrétnější nápovědu a podporu k tomuto tématu.
- Pokud se při volání Microsoft graphu aplikace dostanou **chyby autorizace 401 nebo 403** , vyberte v části **získání chyby odepření přístupu (autorizace)** kategorii Microsoft Graph API pro získání přesnější nápovědy a podpory k tomuto tématu.

**Chci používat Microsoft Graph, ale nevíte, kde začít**

Další informace o aplikaci Microsoft Graph naleznete v tématech:

- [Přehled aplikace Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Základní informace o správě identit a přístupu v Microsoft graphu](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začínáme s vytvářením aplikací Microsoft Graph](https://docs.microsoft.com/graph/)
- **Průzkumník Microsoft graphu** – testování rozhraní Microsoft Graph API v tenantovi nebo ukázkovém tenantovi

**Chci používat Microsoft Graph, ale podporuje rozhraní API v adresáři verze 1.0?**

Doporučeným rozhraním API pro správu adresářů, identit a přístupu je Microsoft Graph. V grafu Azure AD a v Microsoft graphu je ale pořád pár mezer. Přečtěte si následující články, které by měly zvýraznit nejaktuálnější rozdíly, které vám umožní váš výběr:

- [Rozdíly mezi typy zdrojů v Azure AD graphu a Microsoft graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdíly mezi vlastnostmi v Azure AD graphu a Microsoft graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdíly mezi metodami v Azure AD a Microsoft graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Při dotazování objektu *uživatele* chybí mnoho jeho vlastností**

`GET https://graph.microsoft.com/v1.0/users` Vrátí jenom 11 vlastností, protože Microsoft Graph automaticky vybere výchozí sadu *uživatelských* vlastností, které se mají vrátit. Pokud potřebujete další vlastnosti *uživatelů* , vyberte pomocí $Select vlastnosti, které aplikace potřebuje. Vyzkoušejte nejprve v **aplikaci Microsoft Graph Explorer** .

**Některé hodnoty vlastností uživatele jsou *prázdné* , i když vím, že jsou nastavené.**

Nejpravděpodobnější vysvětlení je, že aplikaci bylo udělené oprávnění *User. ReadBasic. All* . To umožňuje aplikaci číst omezenou sadu uživatelských vlastností a vracet tak všechny ostatní vlastnosti jako hodnoty null, a to i v případě, že byly dříve nastavené. Zkuste udělit oprávnění *uživatele aplikace. Read. All* .

Další informace najdete v článku [uživatelská oprávnění aplikace Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Mám potíže s použitím parametrů dotazu OData k filtrování dat v mých žádostech**

Zatímco Microsoft Graph podporuje široký rozsah parametrů dotazu OData, mnohé z těchto parametrů nejsou plně podporované adresářovými službami (prostředky, které dědí z *directoryObject*) v Microsoft graphu. Stejná omezení, která byla uložena v Azure AD grafu ve většině částí aplikace Microsoft Graph:

1. **Nepodporované**: $count, $search a *$Filter na hodnoty null* nebo *NOT NULL*
2. **Nepodporované**: $Filter na určitých vlastnostech (viz témata o zdrojích, na kterých se dají filtrovat vlastnosti)
3. **Nepodporované**: stránkování, filtrování a řazení najednou
4. **Nepodporuje se**: filtrování podle vztahu. Můžete například najít všechny členy technické skupiny, kteří jsou ve Velké Británii.
5. **Částečná podpora**: $OrderBy pro *uživatele* (jenom DisplayName a userPrincipalName) a *skupiny*
6. **Částečná podpora**: $Filter (podporuje jenom *EQ*, *StartsWith* *nebo* a *omezená* *jakákoli*), $expand (rozbalení relací jednoho objektu vrátí všechny relace, ale rozbalování relací objektů je omezené)

Další informace najdete v tématu [přizpůsobení odpovědí pomocí parametrů dotazu](https://docs.microsoft.com/graph/query-parameters).

**Rozhraní API, které já zavolám nefunguje – kde můžu dělat další testování?**

**Průzkumník Microsoft graphu** – otestujte rozhraní API Microsoft graphu ve vašem tenantovi nebo ukázkovém tenantovi a podívejte se také na **Ukázkové dotazy** v aplikaci Microsoft Graph Explorer.

**Když se dotazovat na data, zdá se, že mám nekompletní sadu dat**

Pokud vytváříte dotazování na kolekci (například *Uživatelé*), používá Microsoft Graph limit stránek na straně serveru, takže výsledky jsou vždycky vráceny s výchozí velikostí stránky. Aplikace by měla vždy očekávat, že budou stránky ze sběru vrácené službou.

Další informace najdete tady:

- [Doporučené postupy pro Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Stránkování dat aplikace Microsoft Graph ve vaší aplikaci](https://docs.microsoft.com/graph/paging)

**Moje aplikace je moc pomalá a zároveň zobrazuje omezení. Jaká vylepšení můžu dělat?**

V závislosti na tom, jaký máte váš scénář, máte k dispozici nejrůznější různé možnosti, díky kterým bude aplikace pracovat, a v některých případech méně náchylné k omezení služby (při provádění příliš mnoha hovorů).

Více k tomu najdete tady:

- [Doporučené postupy pro Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Žádosti o dávkové zpracování](https://docs.microsoft.com/graph/json-batching)
- [Sledování změn v rozdílovém dotazu](https://docs.microsoft.com/graph/delta-query-overview)
- [Upozornění na změny prostřednictvím webhooků](https://docs.microsoft.com/graph/webhooks)
- [Pokyny pro omezení](https://docs.microsoft.com/graph/throttling)

**Kde najdu Další informace o chybách a známých problémech?**

- [Informace o chybové odezvě Microsoft graphu](https://docs.microsoft.com/graph/errors)
- [Známé problémy s Microsoft graphem](https://docs.microsoft.com/graph/known-issues)

**Kde můžu zkontrolovat stav dostupnosti služeb a připojení?**

Dostupnost a připojení základních služeb, ke kterým lze získat přístup pomocí aplikace Microsoft Graph, může ovlivnit celkovou dostupnost a výkon aplikace Microsoft Graph.

- Pro stav služby Azure Active Directory zkontrolujte stav služby **Security + Identity** uvedené na [stránce Stav Azure](https://azure.microsoft.com/status/).
- V případě služeb Office, které přispívají do aplikace Microsoft Graph, zkontrolujte stav služeb uvedených na [řídicím panelu stavu služby Office](https://portal.office.com/adminportal/home#/servicehealth).
