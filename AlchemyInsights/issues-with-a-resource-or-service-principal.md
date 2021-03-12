---
title: Problémy s hlavním zdrojem nebo hlavním objektem služby
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713446"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problémy s hlavním zdrojem nebo hlavním objektem služby

1. Pokud právě začínáte, objekty instanční aplikace a služby v [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) popisují registraci aplikací, objekty aplikace a objekty služby v Azure Active Directory: co to jsou, jak se používají a jak spolu souvisejí. Scénář s příkladem více tenantů také znázorňuje vztah mezi objektem aplikace a odpovídajícími objekty hlavního názvu služby.
2. Další informace o relaci mezi aplikacemi a objekty zabezpečení služby najdete v čtení aplikací a objektů hlavního názvu služby v [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Postupy:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Použití portálu k vytvoření aplikace a hlavního názvu služby Azure AD, které mají přístup k prostředkům, vám ukáže, jak vytvořit novou aplikaci a hlavní název služby Azure Active Directory (Azure AD), který se může použít s řízením přístupu založeného na rolích.
4. S hlavním [rozhraním API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)služby můžete programově spravovat instance aplikací a řídit, co aplikace může dělat v rámci vašeho tenanta.
5. [Hlavní název služby typu zdroje](https://docs.microsoft.com/graph/api/resources/serviceprincipal) uvádí všechny vlastnosti a metody pro typ zdroje hlavní atribut služby.
6. [Rozdíly typů zdrojů mezi Azure AD Graph a Microsoft Graphem zvýrazňují](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) rozdíly mezi zdroji Azure AD Graph a Microsoft Graph. Zobrazuje zdroje, které mají jiné názvy nebo nejsou dostupné. také zvýrazní zdroje, které jsou dostupné v beta verzi Microsoft Graphu, ale ne ve verzi v1.0.

**Problémy s uživateli s hosty**

- [Rychlý start:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Přidání uživatelů hosta do adresáře na portálu Azure Portal ukazuje, jak přidat nového uživatele hosta do adresáře Azure AD přes portál Azure Portal, poslat pozvánku a vidět, jak vypadá proces uplatnění pozvánky hosta.
- [Kurz: Vytvoření toku uživatelů v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) ukazuje, jak vytvořit některé doporučené toky uživatelů pomocí portálu Azure Portal. Pokud hledáte informace o tom, jak v aplikaci nastavit přihlašovací údaje pro heslo vlastníka prostředků (ROPC), podívejte se na postup konfigurace přihlašovacích údajů vlastníka prostředku v Azure AD B2C.
