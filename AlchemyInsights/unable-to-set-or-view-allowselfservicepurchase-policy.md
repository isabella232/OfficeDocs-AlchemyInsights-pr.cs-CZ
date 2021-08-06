---
title: Nelze nastavit nebo zobrazit zásadu AllowSelfServicePurchase.
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020185"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nelze nastavit nebo zobrazit zásadu AllowSelfServicePurchase.

Při pokusu o nastavení nebo zobrazení zásad AllowSelfServicePurchase se zobrazí následující chybová zpráva:

*Chyba_zpracování: Nepodařilo se načíst zásady produktu pomocí id_zásady AllowSelfServicePurchase, ErrorMessage – základní připojení bylo uzavřeno: Při odeslání došlo k neočekávané chybě.*

Může to být způsobeno starší verzí tls (Transport Layer Security). Pokud chcete připojit službu MSCommerce, musíte použít TLS 1.2 nebo vyšší.  

Zkuste protokol TLS povolit nebo nastavit na 1.2, ověřit ho a zkusit to znovu.
 1. Na příkazovém řádku PowerShellu (PS C: zadejte následující příkaz, který nastaví protokol \) TLS na verzi 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Ověřte používaný protokol TLS pomocí následujícího příkazu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Podle potřeby opakujte příkazy Získat nebo Aktualizovat.

