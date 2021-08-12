---
title: Zakázání kontroly v síti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7e67a45b6f4d4b18f47ce55a0fde20f826498c5d25c4a6dec4311d8fe4c3735f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928542"
---
# <a name="disable-network-scan"></a>Zakázání kontroly v síti

Kontroly sdílené síťové složky mohou mít vliv na výkon.  Pokud chcete zajistit, aby klient ve výchozím nastavení neskenuje sdílené síťové složky nebo soubory, nakonfigurujte následující nastavení v Windows Defender na **True**:

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles