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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999233"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kvůli problémům s prohlížečem se nedaří přihlásit k Azure (prohlížeč přestane reagovat, neustále se točí, nenačte se atd.)

Na vás může mít dopad výpadku. Zkontrolujte prosím, jestli došlo k probíhajícímu výpadku: [Stav Azure .](https://status.azure.com/status/history/)

Odhlásit se prosím ze všech aktivních relací Azure. Spusťte v soukromém nebo anonymním režimu webového prohlížeče.

Můžete se taky pokusit aktualizovat prohlížeč, použít jiný prohlížeč, odstranit soubory cookie mezipaměti, pokud výše uvedené nefunguje.

Další informace: [Řešení potíží s přihlášením](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nelze získat přístup k předplatným**

Na [portálu Azure Portal](https://portal.azure.com/)se ujistěte, že je v účtu vpravo nahoře vybraný správný adresář Azure.

V Centru [účtů Azure](https://account.windowsazure.com/Subscriptions)zkontrolujte, jestli je použitý účet správcem účtu.

Další informace: [Řešení potíží s nenahledaným předplatným](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Historie fakturace není přístupná.**

Správce účtu musí zajistit, aby se uživatel, který přistupuje k fakturačním informacím, přidal do adresáře Azure Active jako hostující uživatel: Přidání nebo odstranění [nového uživatele](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Uživatel pak musí mít roli globálního správce: [Přiřazení role uživatelům](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Tento příspěvek můžete uživateli udělit přístup k fakturaci pomocí zásad RBAC: [Udělení přístupu k fakturaci](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Doporučené dokumenty**

-   [Nemůžu se přihlásit ke správě předplatného Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)