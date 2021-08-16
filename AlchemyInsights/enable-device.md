---
title: Povolit zařízení
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003468"
---
# <a name="enable-device"></a>Povolit zařízení

**Povolení zařízení pomocí příkazu PowerShell**

Spusťte následující příkazy:

- Získání objektu zařízení: `Get-MsolDevice -Name <Name>`
- Povolení zařízení: `Enable-MsolDevice -DeviceId <DeviceId>`

Další informace o konfiguraci hybridního připojení ve spravovaných doménách najdete v tématu [Konfigurace hybridního připojení.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
