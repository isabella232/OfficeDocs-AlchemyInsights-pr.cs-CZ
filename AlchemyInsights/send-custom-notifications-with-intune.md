---
title: Posílání vlastních oznámení pomocí Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086157"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Jak posílat vlastní oznámení uživatelům spravovaných zařízení s iOSem a Androidem

Vlastní oznámení pro Intune zpracovává aplikace Portál společnosti na zařízení uživatele. Aplikace pak na tomto zařízení vytvoří nabízené oznámení.

Tady jsou požadavky na zařízení pro podporu přijímání vlastních oznámení a aplikace pak vytvoří nabízená oznámení:

- Zařízení musí mít nainstalovanou Portál společnosti aplikaci.  

- Zařízení musí aplikaci Portál společnosti odesílat nabízená oznámení. Když je aplikace nainstalovaná nebo aktualizovaná, zobrazí uživateli výzvu k povolení oznámení.

- Zařízení s Androidem musí mít nainstalované služby Google Play.

- Zařízení musí být zaregistrované v Intune.

Další informace včetně toho, jak poslat zprávu, najdete v [dokumentaci k funkcím](https://docs.microsoft.com/intune/custom-notifications).
