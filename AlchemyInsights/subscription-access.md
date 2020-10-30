---
title: Přístup k předplatnému
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807224"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nejde se přihlásit do Azure kvůli problémům s prohlížečem (prohlížeč se zablokuje, nenačte se atd.).

Pravděpodobně bude ovlivněn výpadek. Zkontrolujte, jestli se nejedná o probíhající výpadek: [stav Azure](https://status.azure.com/status/history/).

Odhlaste se ze všech aktivních relací Azure. Začněte v soukromém nebo prohlížečinové režimu webového prohlížeče.

Můžete se taky pokusit aktualizovat prohlížeč, použít jiný prohlížeč, odstranit soubory cookie mezipaměti, pokud dřív nefunguje.

Další informace: [řešení potíží s přihlašováním](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nelze získat přístup k předplatným**

Na [portálu Azure](https://portal.azure.com/)se ujistěte, že je v pravém horním rohu vybraná správná složka Azure.

V [centru účtů Azure](https://account.windowsazure.com/Subscriptions)zkontrolujte, jestli je použitý účet správcem účtu.

Další informace: [řešení potíží s žádným předplatným](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nelze získat přístup k historii fakturace**

Správce účtu musí zajistit, aby uživatel, který přistupuje k fakturačním informacím, přidal do služby Azure Active Directory jako hosta uživatele: [Přidání nebo odstranění nového uživatele](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Uživatel pak musí mít roli globálního správce: [přiřazení role uživatelům](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Publikovat: uživateli je možné udělit fakturační přístup pomocí zásad RBAC: [udělte přístup k fakturaci](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Doporučené dokumenty**

-   [Nemůžu se přihlásit ke správě svého předplatného Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)