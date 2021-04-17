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
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826084"
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

