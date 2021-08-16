---
title: Oznámení AAD Připojení
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
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097299"
---
# <a name="notification-aad-connect"></a>Oznámení AAD Připojení

- Ujistěte se, že máte oprávnění k provedení operace. Globální správci mají ve výchozím nastavení přístup. K delegování [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) oprávnění k registraci přispěvateli můžete použít řízení přístupu založeného na rolích.
- Zajistěte, aby byly povolené požadované koncové body a nebyly blokovány kvůli bráně firewall. Podrobnosti najdete v tématu [Požadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrace může selhat, protože odchozí komunikace podléhá kontrole SSL přes síťovou vrstvu.
- Ujistěte se, že jste ověřili nastavení oznámení pro Azure AD Připojení Health a zkontrolujte nastavení. Informace o konfiguraci nastavení oznámení pro oznámení Azure AD Připojení Stavu najdete v této [příručce.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Další informace o sestavě synchronizace AAD Připojení stavu a o tom, jak ji stáhnout, najdete v tématu Sestava synchronizace [na úrovni objektů](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Řešení potíží s upozorněními na stav služby AAD Připojení postupujte podle příručky pro řešení potíží s upozorněními na stavová data [AAD Připojení Stav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a nejčastější dotazy najdete v článku Časté otázky týkající se instalace [AAD Připojení Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
