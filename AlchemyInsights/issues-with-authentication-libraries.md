---
title: Problémy s knihovnami ověřování
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54027997"
---
# <a name="issues-with-authentication-libraries"></a>Problémy s knihovnami ověřování

1. [Microsoft identity platform knihovny ověřování uvádí](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) knihovny klientů a middlewarů podporované společností Microsoft a kompatibilní.
2. Knihovna MSAL (Microsoft Authentication Library) podporuje několik [toků ověřování](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pro použití v různých scénářích aplikací.
3. Pokud chcete ověřit a získat tokeny, inicializujete novou veřejnou nebo důvěrnou klientskou aplikaci v kódu. Při inicializaci klientské aplikace v knihovně msal (Microsoft Authentication Library) můžete nastavit několik možností konfigurace. Další informace najdete v tématu [Možnosti konfigurace aplikace](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Ukončení podpory knihovny Azure Active Directory ověřování (ADAL) a rozhraní API služby Azure AD Graph (AAD Graph)**

**Od 30. června 2020** už nebudeme přidávat žádné nové funkce do ADAL a Azure AD Graph. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.

**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a už nebudeme poskytovat technickou podporu ani aktualizace zabezpečení.

Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po této době fungovat, ale nebudou dostávat technickou podporu ani *aktualizace zabezpečení*.

Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graph azure ad.

**Migrace ADAL**

Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.

Pokud používáte aplikace Microsoft, věrte, že Microsoft do konečného termínu ukončení podpory migruje své aplikace na MSAL, aby se zajistilo, že budou mít prospěch z průběžného zabezpečení a vylepšení funkcí společnosti MSAL.

Další informace najdete tady:

1. [Přečtěte si časté otázky k ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informace o tom, jak migrovat aplikace na základě platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Pokud potřebujete pomoc s pochopením, které z vašich aplikací používají ADAL, doporučujeme zkontrolovat zdrojový kód všech aplikací a případně kontaktovat poskytovatele internetových služeb nebo poskytovatelů aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají Azure AD Graph, postupujte podle našich pokynů k migraci [aplikací Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)na Microsoft Graph .

1. [Náš kontrolní seznam migrace poskytuje základní informace.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací. Podpora Microsoftu vám taky může poskytnout seznam všech využití služby AAD Graph ve vašem tenantovi.
3. Aby vaše aplikace přistupovat k datům v microsoft Graph, musí mu uživatel nebo správce udělit správná oprávnění prostřednictvím procesu souhlasu. Odkaz [microsoft Graph oprávnění](https://docs.microsoft.com/graph/permissions-reference) uvádí oprávnění přidružená ke každé hlavní sadě rozhraní Microsoft Graph API. Obsahuje také pokyny k používání oprávnění.
