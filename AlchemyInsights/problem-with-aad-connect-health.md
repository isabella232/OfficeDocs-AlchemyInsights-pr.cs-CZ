---
title: Problém se stavem služby AAD Connect
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481151"
---
# <a name="problem-with-aad-connect-health"></a>Problém se stavem služby AAD Connect

- Ujistěte se, že máte oprávnění k provádění operace. Ve výchozím nastavení mají přístup globální správci. Navíc můžete pomocí ovládacího prvku přístupu [založeného na](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) rolích delegovat oprávnění k registraci přispěvatele.
- Ujistěte se, že jsou povolené požadované koncové body a nezablokují se kvůli bráně firewall. Podrobnosti najdete v části [požadavky.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registrace může selhat, pokud se odchozí komunikace podrobuje kontrole SSL síťové vrstvě.
- Zkontrolujte, že jste ověřili nastavení oznámení pro Azure AD Connect Health. Zkontrolujte prosím nastavení. Tento [průvodce vám](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pomůže pochopit, jak nakonfigurovat nastavení oznámení pro upozornění na stav služby Azure AD Connect.
- Další informace o sestavě synchronizace služby AAD Connect Health a o tom, jak ji stáhnout, najdete v [sestavě synchronizace na úrovni objektů.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Pokud chcete vyřešit upozornění na stav služby AAD Connect, postupujte podle pokynů průvodce pro řešení potíží s upozorněními na aktualizace dat [služby AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a nejčastějšími otázkami k instalaci najdete v článku Časté otázky týkající se instalace služby [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
