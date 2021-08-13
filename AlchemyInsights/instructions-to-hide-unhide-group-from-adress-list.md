---
title: Pokyny ke skrytí nebo zobrazení skupiny ze seznamu adres
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926238"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrytí Microsoft 365 skupiny ze seznamu adres (GAL)

Pokud chcete skrýt Microsoft 365 skupiny adres (GAL) Exchange klientů (například Outlook nebo OWA), použijte v prostředí EXO následující příkaz:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Pokud chcete skrýt Microsoft 365 skupiny, aby se Exchange klientům, použijte následující příkaz v prostředí EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

