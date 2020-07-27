---
title: Zásady ochrany aplikací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423430"
---
# <a name="application-protection-policy"></a>Zásady ochrany aplikací

Pokud se zásadami ochrany aplikací (APP) začínáte, podívejte se na [přehled zásad ochrany aplikací](https://docs.microsoft.com/intune/apps/app-protection-policy).

Pokud chcete začít používat aplikaci APP, přečtěte [si téma Jak vytvořit a přiřadit zásady ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies).

Požadavky zásad ochrany aplikací:

- Uživatel má licenci Intune nebo EMS.
- Uživatel patří do skupiny, na kterou se zaměřují zásady ochrany aplikací.
- K chráněným aplikacím na zařízení je přihlášen pouze jeden podnikový uživatel.
- Aplikace implementovala [intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Seznam aplikací, které sadu SDK podporují, najdete v tématu [Chráněné aplikace Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Zásady platí poté, co se uživatel, který splňuje výše uvedené požadavky, přihlásí do aplikace s povolenou intune SDK. Nejjednodušší způsob, jak zjistit, zda je použita zásada je tím, že vyžaduje, aby uživatel nastavit pin v zásadách. 

Další informace najdete tady:

[Nejčastější dotazy k řešení potíží s aplikací APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Jak ověřit nastavení zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Principy časování doručování zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Jak sledovat zásady ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies-monitor)