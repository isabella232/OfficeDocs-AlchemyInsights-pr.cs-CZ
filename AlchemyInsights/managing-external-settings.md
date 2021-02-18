---
title: Správa externích nastavení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294169"
---
# <a name="managing-external-settings"></a>Správa externích nastavení

**Oznámení**

- Od 4. ledna 2021 se od Googlu ode dne 4. ledna [2021 odepíše podpora přihlášení WebView.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support) Otestujte, jestli se na vaše aplikace vliv mají, a to podle pokynů Googlu pro testování kompatibility.
- Při přihlašování uživatelů pomocí spotřebitelských účtů Google nezapomeňte použít webové zobrazení systému nebo prohlížeč systému.

**Správa nastavení pozvánek**

Potvrďte, že jste [nakonfigurovali nastavení externí spolupráce tak,](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) aby se příslušnými lidmi mohly posílat pozvánky.

**Správa přístupových oprávnění uživatelů hosta**

1. Globální správci mohou spravovat přístupová oprávnění hostů v adresáři prostřednictvím portálu Azure Portal nakonfigurováním oprávnění pro přístup hostů na stránce Nastavení externí spolupráce. [Přečtěte si další informace o tomto nastavení.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)
2. Pokud chcete, aby vaši hosté měli přístup k aplikacím, jako je Teams nebo SharePoint, potvrďte, že jste je nakonfigurovali tak, aby přístup hostů povoloval. Přečtěte si další informace [o nastavení teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) a [SharePointu.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurace pozvánek:**

- [Povolte externí spolupráci S2B a spravujte, kdo může zvat hosty.](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Povolit nebo blokovat pozvánky uživatelům z určitých organizací](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurace povolených zprostředkovatelů identity:**

- [Google Federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Přímá federace](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ověření e-mailového hesla v jednom e-mailu](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
