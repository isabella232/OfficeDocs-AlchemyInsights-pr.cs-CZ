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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014750"
---
# <a name="delete-or-restore-applications"></a>Odstranění nebo obnovení aplikací

**Odstranění aplikace z vašeho tenanta Azure AD**:

1. Na **portálu Azure AD** vyberte **aplikace Enterprise**. Pak vyhledejte a vyberte aplikaci, kterou chcete odstranit.
2. V levém podokně klikněte v části **Spravovat** na **vlastnosti**.
3. Vyberte **Odstranit** a pak kliknutím na **Ano** potvrďte, že chcete aplikaci odstranit z vašeho tenanta Azure AD.

Další informace o odstranění aplikace najdete v tématu [rychlý automat: odstranění aplikace z vašeho tenanta Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

V PowerShellu rutina [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) odebere konfigurace proxy aplikací z konkrétní aplikace v Azure Active Directory a může ji úplně odstranit, pokud je zadaná.

**Odstraněnou aplikaci můžete obnovit** pomocí PowerShellu. Jakmile je aplikace, kterou chcete obnovit, označena, můžete ji obnovit pomocí funkce [obnovit – AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
