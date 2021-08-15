---
title: Problémy s vývojem aplikací s rozhraními API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013453"
---
# <a name="issues-developing-applications-with-apis"></a>Problémy s vývojem aplikací s rozhraními API

Pokud chcete začít rozhraní Azure Active Directory Graph API, podívejte se na úvodní příručku k [rozhraní Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) nebo si prohlédněte interaktivní referenční dokumentaci k rozhraní Azure AD Graph [API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Ukončení podpory knihovny Azure Active Directory ověřování (ADAL) a rozhraní API služby Azure AD Graph (AAD Graph)**

**Od 30. června 2020** už nebudeme přidávat žádné nové funkce do ADAL a Azure AD Graph. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.

**Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a už nebudeme poskytovat technickou podporu ani aktualizace zabezpečení.

Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po tomto datu fungovat, ale nebudou mít technickou podporu ani aktualizace zabezpečení.

Aplikace používající Azure AD Graph po této době už nemusí dostávat odpovědi z koncového bodu Azure AD Graph azure ad.

**Migrace ADAL**

Doporučujeme aktualizovat na knihovnu [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.

Pokud používáte aplikace Microsoftu, věděli jste, že Microsoft do konečného termínu ukončení podpory migruje své aplikace na MSAL, což zajistí, že budou mít prospěch z průběžného zabezpečení a vylepšení funkcí společnosti MSAL.

1. [Přečtěte si časté otázky k ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Přečtěte si, jak migrovat aplikace na platformě.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Pokud potřebujete pomoc s pochopením, které z vašich aplikací používají ADAL, doporučujeme zkontrolovat zdrojový kód všech aplikací a případně kontaktovat poskytovatele internetových služeb nebo poskytovatelů aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.

**Migrace AAD Graphu**

U aplikací, které používají Azure AD Graph, postupujte podle našich pokynů k migraci [aplikací Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)do Microsoft Graph .

1. [Základní informace najdete v našem kontrolním seznamu migrace](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Aplikace používající AAD Graph najdete na registračním portálu aplikace Azure. Doporučujeme, abyste zkontrolovali zdrojový kód všech svých aplikací, a pokud to bude možné, kontaktovali všechny nezávislé dodavatele softwaru nebo poskytovatele aplikací. Podpora Microsoftu vám taky může poskytnout seznam všech využití služby AAD Graph ve vašem tenantovi.
1. Aby vaše aplikace přistupovat k datům v microsoft Graph, musí mu uživatel nebo správce udělit správná oprávnění prostřednictvím procesu souhlasu. Odkaz [microsoft Graph oprávnění](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) uvádí oprávnění přidružená ke každé hlavní sadě rozhraní Microsoft Graph API. Obsahuje také pokyny k používání oprávnění.
