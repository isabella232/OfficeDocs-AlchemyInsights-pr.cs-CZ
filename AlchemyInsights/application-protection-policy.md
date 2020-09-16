---
title: Zásady ochrany aplikací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716886"
---
# <a name="application-protection-policy"></a>Zásady ochrany aplikací

Pokud se zásadou ochrany aplikací (aplikace) nepracujete, podívejte se na [Přehled zásad ochrany aplikací](https://docs.microsoft.com/intune/apps/app-protection-policy).

Pokud chcete začít používat aplikaci, přečtěte si [článek Jak vytvořit a přiřadit zásady ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies).

Požadavky na zásady ochrany aplikací:

- Uživatel má licenci Intune nebo EMS.
- Uživatel patří do skupiny, která je cílová v zásadách ochrany aplikací.
- Do chráněných aplikací na zařízení se přihlásí jenom jeden podnikový uživatel.
- Aplikace implementovala [sadu Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Seznam aplikací, které podporují sadu SDK, najdete v tématu [Microsoft Intune Protected Apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Zásady platí, když uživatel, který splňuje výše uvedené požadavky, podepíše do aplikace Intune s podporou sady SDK. Nejjednodušším způsobem, jak zjistit, jestli je zásada použitá, je to, když uživatel nastavil v zásadě PIN kód. 

Další informace najdete tady:

[Časté otázky k aplikaci MAM a nejčastější dotazy](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Jak ověřit nastavení zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Principy časování doručení zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Sledování zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies-monitor)