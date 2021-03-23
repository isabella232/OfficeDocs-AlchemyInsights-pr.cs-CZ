---
title: Práce s knihovnami ověřování
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035015"
---
# <a name="working-with-authentication-libraries"></a>Práce s knihovnami ověřování

Pokud chcete vyřešit problém s knihovnou MSAL (Microsoft Authentication Library), proveďte následující doporučené kroky:

1. **Práce s rozhraním MSAL**: Knihovny ověřování [na platformě identit Microsoftu](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – tento článek ukazuje podporu knihovny microsoftového ověřování pro několik typů aplikací. Obsahuje odkazy na zdrojový kód knihovny. kde získat balíček pro projekt aplikace; a jestli knihovna podporuje přihlášení uživatele (ověřování), přístup k chráněným webovým rozhraním API (autorizace) nebo obojí.

2. **Poradce při potížích** s ověřováním: Funkce MSAL podporuje několik toků ověřování pro použití v různých scénářích aplikací. V závislosti na tom, jak je vaše klientská aplikace vytvořená, může msal použít jeden nebo více toků ověřování podporovaných platformou identit Microsoftu. Tyto toky mohou vytvářet několik typů tokenů a autorizačních kódů a vyžadovat různé tokeny, aby fungovaly.

3. **Přístupové tokeny:** [Přístupové tokeny platformy microsoftu](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – zjistěte, jak může rozhraní API ověřovat a používat deklarace identity uvnitř přístupového tokenu. Veškerá dokumentace v tomto článku, s výjimkou případů uvedených, platí jenom pro tokeny vydané pro rozhraní API, která jste zaregistrovali. Nevztahuje se na tokeny vydané pro rozhraní API vlastněné společností Microsoft a tyto tokeny se nedávají použít k ověření, jak bude platforma identit Microsoft vydávat tokeny pro rozhraní API, které vytvoříte.

**Ukončení podpory knihovny ověřování služby Azure Active Directory (ADAL)**

- **Od 30. června 2020** už nebudeme přidávat žádné nové funkce do ADAL a Azure AD Graphu. Budeme dál poskytovat technickou podporu a aktualizace zabezpečení, ale už nebudeme poskytovat aktualizace funkcí.
- **Od 30. června 2022** ukončíme podporu pro ADAL a Azure AD Graph a už nebudeme poskytovat technickou podporu ani aktualizace zabezpečení.
- Aplikace, které používají ADAL ve stávajících verzích operačního systému, budou i po této době fungovat, ale nebudou dostávat technickou podporu ani *aktualizace zabezpečení*.
- Aplikace používající Azure AD Graph po této době už nemusí přijímat odpovědi z koncového bodu Azure AD Graphu.

**Migrace ADAL**

- Doporučujeme aktualizovat na msal, který má nejnovější funkce a aktualizace zabezpečení.
- Pokud používáte aplikace Microsoft, věrte, že Microsoft do konečného termínu ukončení podpory migruje své aplikace na MSAL, takže budou mít prospěch z průběžného zabezpečení a vylepšení funkcí msal.

1. [Přečtěte si časté otázky k ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Přečtěte si, jak migrovat aplikace na platformě.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Pokud po přečtení příručky pro platformu vaší aplikace máte další otázky, můžete příspěvek na [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) se značkou [azure-ad-adal-deprecation] nebo otevřít problém v úložišti GitHubu knihovny. Odkazy [na repo](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) knihovny najdete v části Jazyky a rámce v článku přehledu **MSAL.**
4. **Pokud potřebujete pomoct s pochopením, které aplikace používají ADAL,** doporučujeme zkontrolovat zdrojový kód všech aplikací. Pokud je to možné, můžete kontaktovat nezávislé dodavatele softwaru (ISV) nebo poskytovatele aplikací. Seznam všech aplikací na vašem tenantovi, které nejsou od Microsoftu a používají ADAL, vám může poskytnout podpora Microsoftu.







