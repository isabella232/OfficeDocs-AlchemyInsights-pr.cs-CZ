---
title: Odstranění nebo obnovení aplikací
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102564"
---
# <a name="delete-or-restore-applications"></a>Odstranění nebo obnovení aplikací

**Odstranění aplikace z tenanta Azure AD**:

1. Na portálu **Azure AD vyberte** Enterprise **aplikací.** Pak najděte a vyberte aplikaci, kterou chcete odstranit.
2. V části **Manage** (Spravovat) v levém podokně vyberte **Properties (Vlastnosti).**
3. Vyberte **Odstranit** a pak vyberte **Ano** a potvrďte, že chcete aplikaci odstranit ze svého tenanta Azure AD.

Další informace o tom, jak odstranit aplikaci, najdete v tématu Rychlý start: Odstranění aplikace z tenanta [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

V PowerShellu rutina [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) odebere konfigurace proxy aplikací z konkrétní aplikace v Azure Active Directory a může ji úplně odstranit, pokud je zadaná.

Odstraněnou **aplikaci můžete obnovit pomocí** PowerShellu. Jakmile bude aplikace, kterou chcete obnovit, identifikována, můžete ji obnovit pomocí [funkce Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
