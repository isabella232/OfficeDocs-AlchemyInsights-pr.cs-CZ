---
title: Problémy se zdrojem nebo hlavním objektem služby
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028069"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problémy se zdrojem nebo hlavním objektem služby

1. Pokud právě začínáte, application and [service principal](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) objects in Azure Active Directory describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other. Příklad scénáře s více tenanty je také prezentován tak, aby ilustroval vztah mezi aplikačním objektem aplikace a odpovídajícími hlavními objekty služby.
2. Další informace o relaci mezi aplikacemi a objekty služby najdete v části Čtení aplikací a hlavních objektů služby [v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Postupy:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Pomocí portálu můžete vytvořit aplikaci a hlavní objekt služby Azure AD, který má přístup k prostředkům, ukazuje, jak vytvořit novou aplikaci Azure Active Directory (Azure AD) a hlavní objekt služby, který se může použít s řízením přístupu založeném na rolích.
4. S hlavním [rozhraním API služby](https://docs.microsoft.com/graph/api/resources/serviceprincipal)můžete programově spravovat instance aplikací a řídit, co aplikace může dělat ve vašem tenantovi.
5. [Typ zdroje servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) uvádí všechny vlastnosti a metody pro typ zdroje servicePrincipal.
6. [Rozdíly typu prostředků mezi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) zvýrazňují rozdíly mezi prostředky Azure AD Graph a Microsoft Graph zdrojů. Zobrazuje zdroje, které mají jiné názvy nebo nejsou dostupné. Také zvýrazní zdroje dostupné v beta verzi Microsoftu Graph ale ne ve verzi v1.0.

**Problémy s uživateli hosta**

- [Rychlý start:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Přidání hosta do adresáře na portálu Azure portal vám ukáže, jak přidat nového hosta do adresáře Azure AD prostřednictvím portálu Azure Portal, poslat pozvánku a podívat se, jak vypadá proces uplatnění pozvánky hosta.
- [Kurz: Vytvoření toků uživatelů v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) vám ukáže, jak vytvořit některé doporučené toky uživatelů pomocí portálu Azure Portal. Pokud hledáte informace o tom, jak nastavit tok přihlašovacích údajů pro heslo vlastníka prostředku (ROPC) ve vaší aplikaci, podívejte se na informace v tématu Konfigurace toku přihlašovacích údajů pro heslo vlastníka prostředku v Azure AD B2C.
