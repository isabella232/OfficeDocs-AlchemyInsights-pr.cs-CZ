---
title: Problém s AAD Připojení Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923745"
---
# <a name="problem-with-aad-connect-health"></a>Problém s AAD Připojení Health

- Ujistěte se, že máte oprávnění k provedení operace. Globální správci mají ve výchozím nastavení přístup. K delegování [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) oprávnění k registraci přispěvateli můžete použít řízení přístupu založeného na rolích.
- Zajistěte, aby byly povolené požadované koncové body a nebyly blokovány kvůli bráně firewall. Podrobnosti najdete v tématu [Požadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrace může selhat, protože odchozí komunikace podléhá kontrole SSL přes síťovou vrstvu.
- Ujistěte se, že jste ověřili nastavení oznámení pro Azure AD Připojení Health. Zkontrolujte prosím nastavení. Tato [příručka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vám pomůže pochopit, jak nakonfigurovat nastavení oznámení pro oznámení o stavu Připojení Azure AD.
- Další informace o sestavě synchronizace AAD Připojení stavu a o tom, jak ji stáhnout, najdete v tématu Sestava synchronizace [na úrovni objektů](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Pokud chcete vyřešit potíže s upozorněními na stav služby AAD Připojení, postupujte podle příručky pro řešení potíží s upozorněními na stav a upozorněními na stav a nejčastější dotazy najdete v článku Časté otázky k instalaci A [Připojení AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) [Připojení Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
