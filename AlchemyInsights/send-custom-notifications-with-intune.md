---
title: Odesílání vlastních oznámení pomocí Intune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720639"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Jak posílat vlastní upozornění uživatelům spravovaných zařízení s iOS a Androidem

Vlastní oznámení o Intune zpracovává aplikace Portál společnosti na zařízení uživatele. Aplikace potom vytvoří nabízené oznámení na tomto zařízení.

Níže jsou požadavky na zařízení, které podporují přijímání vlastních oznámení, a pro aplikaci pak vytvoří nabízené oznámení:

- Na zařízení musí být nainstalovaná aplikace Portál společnosti.  

- Zařízení musí povolit aplikaci Portál společnosti odesílat nabízená oznámení. Když se aplikace nainstaluje nebo aktualizuje, vyzve uživatele k povolení oznámení.

- Zařízení s Androidem musí být nainstalovaná služba Google Play.

- Zařízení musí být zaregistrované s Intune.

Další informace včetně odesílání zpráv najdete v [dokumentaci k funkcím](https://docs.microsoft.com/intune/custom-notifications).
