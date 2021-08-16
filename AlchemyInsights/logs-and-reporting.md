---
title: Protokoly a vytváření sestav
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
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067005"
---
# <a name="logs-and-reporting"></a>Protokoly a vytváření sestav

[Azure Active Directory odpovědi na](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) časté otázky týkající se vytváření sestav Azure Active Directory (Azure AD). Další informace najdete v tématu [Azure Active Directory vytváření sestav](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**Řešení problémů s auditem**

1. Pokud máte problémy s některými aktivitami auditování a chybějící aktivita je v tomto [seznamu,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)zapište lístek podpory.
2. Pokud máte problémy s zobrazením protokolů auditování ve vašem tenantovi, zapište lístek podpory.
3. Pokud se vaše aktivity auditování na portálu Azure Portal nezobrazují okamžitě, podívejte se na informace o [latenci](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) a zapište lístek podpory, pokud zpoždění překročí zdokumentovaný latenci.
4. [Uchovávání protokolů aktivit Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. Pokud nevidíte všechny audity pro rozsah dat, který jste vybrali, můžete si z portálu Azure Portal stáhnout až 250 tisíc řádků (seřazených podle nejnovějších). Další informace najdete v tématu [Stažení aktivit auditování](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).

**Řešení problémů s přihlášeními**

1. Data za posledních 30 dní uvidíte jenom v případě, že máte pro svého tenanta licenci Azure AD Premium (P1 nebo P2).
2. Přihlášení jsou dostupná jenom pro Azure AD Premium tenanty. Není k dispozici pro bezplatné nebo základní licencované tenanty.
3. Pokud má váš tenant licenci Premium P1 a nevidíte přihlášení, podívejte se [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) na informace o latenci a zapište lístek podpory, pokud zpoždění překročí zdokumentované latenci.
4. Pokud nevidíte všechna přihlášení pro rozsah dat, který jste vybrali, nezapomeňte, že si můžete stáhnout až 250 tisíc řádků (seřazených podle nejnovějších) přihlášení z portálu Azure Portal. Další informace najdete v tématu [Stažení aktivit přihlášení](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).

**Poradce při potížích se zprávami zabezpečení (Uživatelé s příznakem ohrožení, Rizikové přihlášení)**

1. [Uživatelé označení příznakem pro sestavu zabezpečení rizik](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Risky sign-ins report in the Azure Active Directory portal](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory rizikové události](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
