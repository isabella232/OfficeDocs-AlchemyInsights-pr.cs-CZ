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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013417"
---
# <a name="issues-developing-applications"></a>Problémy s vývojem aplikací

Nejčastější problémy při vytváření aplikací Azure Active Directory (AD), najdete v následujících článcích:

- [Mám potíže s přihlášením k aplikacím jenom v prohlížeči Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nevím, jak změnit výchozí hodnoty životnosti tokenu pro moji aplikaci.](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jsem zmatený ohledně toho, jak funguje souhlas s aplikací.](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nevím, jak udělit oprávnění k aplikaci.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nerozumím rozdílu mezi delegovanou a aplikačními oprávněními](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Ukončení podpory knihovny Azure Active Directory ověřování (ADAL) a rozhraní API služby Azure AD Graph (AAD Graph)***

- Od 30. června 2020 už nebudeme do knihovny Azure Active Directory Authentication Library (ADAL) a rozhraní API Azure AD Graph (AAD Graph) přidávat žádné nové funkce. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.

- Od 30. června 2022 ukončíme podporu pro ADAL a AAD Graph a nebudeme už poskytovat technickou podporu ani aktualizace zabezpečení. Výsledkem této podmínky jsou následující důsledky:

    - Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po tomto datu fungovat, ale nebudou mít technickou podporu ani aktualizace zabezpečení.

    - Aplikace používající AAD Graph po této době už nemusí přijímat odpovědi od koncového bodu AAD Graph AAD.

**Migrace ADAL**

Pokud používáte aplikace Microsoft, doporučujeme aktualizovat na knihovnu MSAL (Microsoft Authentication Library), která obsahuje nejnovější funkce a aktualizace zabezpečení. Toto doporučení je v souvislosti s tím, že Microsoft zahájí proces migrace svých aplikací do MSAL do konečného termínu ukončení podpory. 

Migrace jejích aplikací microsoftem na MSAL zajišťuje, aby tyto aplikace měly prospěch z průběžného zabezpečení a vylepšení funkcí společnosti MSAL.

1. [Přečtěte si časté otázky k ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informace o tom, jak migrovat aplikace na základě platformy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Pokud potřebujete pomoc s pochopením, které z vašich aplikací používají ADAL, doporučujeme zkontrolovat zdrojový kód všech aplikací a případně kontaktovat nezávislé dodavatele softwaru (ISV) nebo poskytovatele aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají AAD Graph, postupujte podle našich pokynů k migraci aplikací AAD Graph na Microsoft Graph:

1. [Základní informace najdete v našem kontrolním seznamu migrace](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme zkontrolovat zdrojový kód všech aplikací a případně kontaktovat nezávislé dodavatele softwaru nebo poskytovatele aplikací. Podpora Microsoftu vám může také poskytnout informace o využití služby AAD Graph ve vašem tenantovi.







