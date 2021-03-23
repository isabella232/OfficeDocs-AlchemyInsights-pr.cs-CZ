---
title: Oznámení AAD Connect
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
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035087"
---
# <a name="notification-aad-connect"></a>Oznámení AAD Connect

- Ujistěte se, že máte oprávnění k provedení operace. Globální správci mají ve výchozím nastavení přístup. K delegování [](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) oprávnění k registraci přispěvateli můžete použít řízení přístupu založeného na rolích.
- Zajistěte, aby byly povolené požadované koncové body a nebyly blokovány kvůli bráně firewall. Podrobnosti najdete v tématu [Požadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrace může selhat, protože odchozí komunikace podléhá kontrole SSL přes síťovou vrstvu.
- Ujistěte se, že jste ověřili nastavení oznámení pro Azure AD Connect Health, a zkontrolujte nastavení. Informace o tom, jak nakonfigurovat nastavení oznámení pro oznámení o stavu služby Azure AD Connect, najdete v této [příručce.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Další informace o sestavě synchronizace stavu připojení služby AAD a o tom, jak ji stáhnout, najdete v tématu Sestava synchronizace [na úrovni objektů](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Řešení potíží s upozorněními na stav připojení služby AAD najdete v průvodci odstraňováním potíží s upozorněními na stav připojení [služby AAD a](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) nejčastějšími dotazy najdete v článku Časté otázky týkající se instalace služby [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
