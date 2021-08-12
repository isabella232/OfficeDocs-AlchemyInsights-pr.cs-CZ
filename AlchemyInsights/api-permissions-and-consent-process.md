---
title: Oprávnění rozhraní API a proces souhlasu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932054"
---
# <a name="api-permissions-and-consent-process"></a>Oprávnění rozhraní API a proces souhlasu

Aby vaše aplikace přistupovat k datům v microsoft Graph, musí mu uživatel nebo správce udělit správná oprávnění prostřednictvím procesu souhlasu. [Odkaz Graph oprávnění microsoftu](https://docs.microsoft.com/graph/permissions-reference) uvádí oprávnění přidružená ke každé hlavní sadě rozhraní Microsoft Graph API. Obsahuje také pokyny k používání oprávnění.

**Nastavení nebo aktualizace hlavního objektu služby**

- [Vytvoření objektu serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – tento článek ukazuje, jak vytvořit nový objekt servicePrincipal.
- [Vytvoření](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) instančního objektu aplikace Azure AD & na portálu – tento článek vám ukáže, jak vytvořit novou aplikaci Azure Active Directory (Azure AD) a hlavní objekt služby, který můžete použít s řízením přístupu založeným na rolích.
- [Aplikace &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) instanční objekty v Azure AD – tento článek popisuje registraci aplikací, aplikační objekty a objekty služby v Azure Active Directory: co jsou, jak se používají a jak se vzájemně souvisejí.

**Přidání nebo aktualizace registrace aplikací a poskytnutí souhlasu správce**

- [Vytvoření registrace aplikace –](https://docs.microsoft.com/graph/api/application-post-applications) tento článek ukazuje, jak vytvořit nový objekt aplikace.
- [Aktualizace registrace aplikace – oprávnění rozhraní API](https://docs.microsoft.com/graph/api/application-update) – tento článek ukazuje, jak aktualizovat vlastnosti objektu aplikace.
- [Poskytnutí souhlasu správce](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – Pro souhlas správce a souhlas obecně požadujeme, aby správce výslovně udělí souhlas.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – kontejner správy rolí pro jednotné definice rolí a přiřazení rolí pro poskytovatele Microsoft 365 RBAC, kteří podporují více objektů zabezpečení a více oborů v jednom přiřazení rolí. Tento typ se liší od *typu zdroje rbacApplication.* Microsoft Intune je příkladem takového poskytovatele RBAC. Přiřazení rolí v Intune může mít matici objektů zabezpečení a matici skupin oborů. **To je v beta verzi, což znamená, že je stále ve vývoji a nedoporučuje se používat v produkční verzi.**
