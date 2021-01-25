---
title: Problémy s vývojem aplikací
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
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974229"
---
# <a name="issues-developing-applications"></a>Problémy s vývojem aplikací

Pokud chcete vyřešit nejběžnější problémy při vytváření aplikací služby Azure Active Directory (AD), podívejte se na následující články:

- [Mám potíže s přihlášením k aplikacím pomocí prohlížeče Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nevím, jak změnit výchozí hodnoty životnosti tokenů pro aplikaci](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Myslím, jak funguje souhlas s aplikací](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nevím, jak udělit oprávnění k aplikaci](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nerozumím rozdílu mezi delegovanými a oprávněními aplikací](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Konec podpory knihovny služby Azure Active Directory (ADAL) a rozhraní API služby Azure AD Graph (graf AAD)** _

- Po zahájení června 2020 nepřidáme do knihovny Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD graphu žádné nové funkce. Budeme dál poskytovat technické podpory a aktualizace zabezpečení, ale nebudete už poskytovat aktualizace funkcí.

- Od června 2022, my vám ukončí podporu pro graf ADAL a AAD a nebude už poskytovat technickou podporu ani aktualizace zabezpečení. V důsledku této podmínky jsou tyto důsledky:

    - Aplikace používající ADAL v existujících verzích OS budou po této době dál fungovat, ale nezískají žádné technické podpory ani aktualizace zabezpečení.

    - Aplikace používající graf AAD po této době už nemusí přijímat odpovědi z koncového bodu grafu AAD.

_ *Migrace**

Pokud používáte aplikace Microsoftu, doporučujeme aktualizovat knihovnu Microsoft Authentication Library (MSAL), která obsahuje nejnovější funkce a aktualizace zabezpečení. Toto doporučení je v souvislosti se společností Microsoft zahajující proces migrace jeho aplikací na MSAL pomocí konečného termínu ukončení podpory. 

Migrace společností Microsoft svých aplikací na MSAL zajišťuje, aby aplikace využily výhody vylepšeného zabezpečení a funkcí MSAL.

1. [Přečtěte si část časté otázky](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informace o migraci aplikací na základě jednotlivých platforem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Pokud potřebujete pomoct s pochopením, které aplikace používají ADAL, doporučujeme, abyste si přezkontrolovali zdrojový kód všech aplikací a případně vyžádejte všechny nezávislé dodavatele softwaru (ISV) nebo poskytovatele aplikací. Podpora Microsoftu vám taky poskytne seznam všech aplikací ADAL, které nejsou od Microsoftu, ve vašem tenantovi.

**Migrace grafu AAD**

U aplikací, které používají diagram AAD, postupujte podle pokynů k migraci aplikací grafu AAD do Microsoft graphu:

1. [Naše kontrolní seznam migrace představuje bod Začínáme](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portál registrace aplikací pro Azure zobrazuje, které aplikace používají graf AAD. Doporučujeme, abyste zkontrolovali všechny zdrojové kódy aplikací a případně Nezávislí poskytovatelé softwaru (ISV) nebo poskytovatelů aplikací. Microsoft Support vám může také poskytnout informace o využití grafu AAD ve vašem tenantovi.







