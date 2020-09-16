---
title: Nelze nastavit nebo zobrazit zásady AllowSelfServicePurchase.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735192"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nelze nastavit nebo zobrazit zásady AllowSelfServicePurchase.

Při pokusu o nastavení nebo zobrazení zásad AllowSelfServicePurchase se zobrazí tato chybová zpráva:

*HandleError: nepovedlo se načíst zásadu produktu s PolicyId AllowSelfServicePurchase, ErrorMessage – nadřízené připojení se zavřelo: došlo k neočekávané chybě při odeslání.*

Příčinou mohou být starší verze protokolu TLS (Transport Layer Security). Abyste mohli připojit službu MSCommerce, musíte používat TLS 1,2 nebo vyšší.  

Zkuste použít následující postup pro povolení/nastavení protokolu TLS na 1,2, ověřte a zkuste to znova.
 1. Na příkazovém řádku PowerShellu (PS C: \) Zadejte následující příkaz pro nastavení protokolu TLS na verzi 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Ověřte používané protokoly TLS pomocí následujícího příkazu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Opakujte pokus o spuštění nebo aktualizaci podle potřeby.

