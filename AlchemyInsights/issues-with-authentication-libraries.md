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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063588"
---
# <a name="issues-with-authentication-libraries"></a>Problémy s knihovnami ověřování

1. [Knihovny ověřování platformy](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identit Microsoft uvádí knihovny klientů a middleware podporovaných a kompatibilními společností Microsoft.
2. Knihovna MSAL (Microsoft Authentication Library) podporuje několik ověřovacích [toků](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pro použití v různých scénářích aplikací.
3. K ověření a získání tokenů můžete v kódu inicializovat novou veřejnou nebo důvěrnou klientskou aplikaci. Při inicializaci klientské aplikace v Knihovně ověřování Microsoft (MSAL) můžete nastavit několik možností konfigurace. Další informace najdete v části [Možnosti konfigurace aplikace.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Ukončení podpory knihovny ADAL (Azure Active Directory Authentication Library) a rozhraní Azure AD Graph API (AAD Graph)**

**Od 30. června 2020** už do ADAL a Azure AD Graphu nebudeme přidávat nové funkce. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.

**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a nebudeme už poskytovat technickou podporu ani aktualizace zabezpečení.

Aplikace používající ADAL ve stávajících verzích operačního systému budou i po této době dál fungovat, ale nebudou dostávat žádné aktualizace technické podpory ani *zabezpečení.*

Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graphu.

**Migrace ADAL**

Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.

Pokud používáte aplikace Microsoftu, věděli jste, že Microsoft ve výchozím nastavení migruje aplikace do systému MSAL do konečného termínu ukončení podpory, takže pro něj bude výhodná průběžná vylepšení zabezpečení a funkcí pro MSAL.

Další informace najdete tady:

1. [Přečtěte si časté otázky k ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informace o tom, jak migrovat aplikace na základě platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Pokud potřebujete pomoct s pochopením, která z vašich aplikací používá ADAL, doporučujeme zkontrolovat si zdrojový kód všech aplikací, a pokud je to možné, kontaktovat některé isVs nebo poskytovatele aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají Azure AD Graph, postupujte podle pokynů k migraci aplikací [Azure AD Graph do Microsoft Graphu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Kontrolní seznam migrace nabízí základní informace.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací. Podpora Microsoftu vám také může poskytnout seznam všech využití AAD Graphu ve vašem tenantovi.
3. Aby vaše aplikace získá přístup k datům v Microsoft Graphu, musí ji uživatel nebo správce udělit správná oprávnění prostřednictvím procesu udělení souhlasu. Odkaz [na oprávnění Microsoft Graphu](https://docs.microsoft.com/graph/permissions-reference) obsahuje oprávnění přidružená k jednotlivým hlavním sadě rozhraní Microsoft Graph API. Obsahuje taky pokyny, jak tato oprávnění používat.
