---
title: Problémy s vývojem aplikací s rozhraním API
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974382"
---
# <a name="issues-developing-applications-with-apis"></a>Problémy s vývojem aplikací s rozhraním API

Pokud chcete začít používat aplikaci Azure Active Directory Graph API, podívejte se na [Příručka Začínáme s API Azure AD graphu](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) nebo si prohlédněte [interaktivní dokumentaci k rozhraní API Azure AD](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Konec podpory knihovny služby Azure Active Directory (ADAL) a rozhraní API Azure AD Graph (graf AAD)**

**Od června 2020** se už nepřidáme žádné nové funkce do grafu ADAL a Azure AD. Budeme dál poskytovat technické podpory a aktualizace zabezpečení, ale nebudete už poskytovat aktualizace funkcí.

**Od června 2022** se vám ukončí podpora pro graf ADAL a Azure AD a nebudete už poskytovat technickou podporu ani aktualizace zabezpečení.

Aplikace používající ADAL v existujících verzích OS budou po této době dál fungovat, ale nezískají žádné technické podpory ani aktualizace zabezpečení.

Aplikace používající graf Azure AD už po této době nemusí přijímat odpovědi z koncového bodu Azure AD.

**ADAL – migrace**

Doporučujeme aktualizovat [knihovnu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), která obsahuje nejnovější funkce a aktualizace zabezpečení.

Pokud používáte Microsoft Apps, je třeba vědět, že společnost Microsoft provádí migraci svých aplikací na MSAL pomocí konečného termínu poskytnutí podpory, což zajistí, že budou těžit ze služby MSAL a vylepšení funkcí.

1. [Přečtěte si téma Nejčastější dotazy](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Přečtěte si, jak migrovat aplikace na jednotlivých platformách](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Pokud potřebujete pomoct s porozuměním, které z vašich aplikací používá ADAL, doporučujeme, abyste si provedli kontrolu všech zdrojových kódů a případně poskytovatelů ISV nebo aplikací. Podpora Microsoftu vám taky poskytne seznam všech aplikací ADAL, které nejsou od Microsoftu, ve vašem tenantovi.

**Migrace grafu AAD**

U aplikací, které používají graf Azure AD, postupujte podle pokynů k migraci [aplikací Graph AD služby Azure do Microsoft graphu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Naše kontrolní seznam migrace představuje bod Začínáme](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portál registrace aplikací pro Azure zobrazuje, které aplikace používají graf AAD. Doporučujeme, abyste zkontrolovali všechny zdrojové kódy aplikací a pokud jsou k dispozici, a pokud je to možné, kontaktujte všechny poskytovatele ISV nebo aplikace. Podpora Microsoftu vám taky poskytne seznam všech použití grafu AAD ve vašem tenantovi.
1. Aby aplikace Access mohla získat přístup k datům v Microsoft graphu, musí ji udělit správnému uživateli nebo správci. [Referenční informace o oprávnění Microsoft graphu](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) zobrazuje oprávnění spojená s jednotlivými hlavními skupinami rozhraní API Microsoft graphu. Poskytuje také pokyny, jak používat oprávnění.
