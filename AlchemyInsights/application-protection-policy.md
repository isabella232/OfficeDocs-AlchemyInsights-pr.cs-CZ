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
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969964"
---
# <a name="application-protection-policy"></a>Zásady ochrany aplikací

Pokud s zásadami ochrany aplikací (APP) ještě nejste, podívejte se na přehled zásad [ochrany aplikací.](https://docs.microsoft.com/intune/apps/app-protection-policy)

Pokud chcete začít používat APP, podívejte [se na postup vytvoření a přiřazení zásad ochrany aplikací.](https://docs.microsoft.com/intune/app-protection-policies)

Požadavky zásad ochrany aplikací:

- Uživatel má licenci Intune nebo EMS.
- Uživatel patří do skupiny, na kterou se zaměřit zásady ochrany aplikací.
- K chráněným aplikacím na zařízení je přihlášen jenom jeden podnikový uživatel.
- Aplikace implementovaná sada [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). Seznam aplikací, které podporují sadu SDK, najdete v Microsoft Intune [chráněných aplikací.](https://docs.microsoft.com/intune/apps-supported-intune-apps)

Zásady platí po tom, co se uživatel, který splňuje výše uvedené požadavky, přihlásí do aplikace s povolenou sadou Intune SDK. Nejjednodušší způsob, jak zjistit, jestli je zásada použitá, je to, že uživatel v zásadách nastaví připínák. 

Další informace najdete tady:

[Nejčastější dotazy k řešení potíží s aplikací APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Jak ověřit nastavení zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Principy časování doručení zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Sledování zásad ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies-monitor)