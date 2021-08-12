---
title: Chyba při odesílání e-mailů blokovaných spamhausem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946705"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Při odesílání e-mailu došlo k chybě: Hostitel klienta je zablokovaný pomocí spamhausu.

IP adresa, která zprávu odeslala, je v seznamu blokových bloků, který vlastní [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Mezi důvody, proč spamhaus blokuje, patří ohrožené účty, ohrožené počítače, které sdílejí veřejnou IP adresu, a zásady poskytovatele internetových služeb. Možné opravy jsou:
  
- U blokovaných příchozích zpráv, na kterých řídíte zdrojový e-mailový server, musíte určit příčinu a odebrat blok z webu Spamhaus.

- U blokovaných příchozích zpráv, u kterých zdrojová IP adresa patří někomu jinému, musí vlastník adresy odebrat blok z webu Spamhaus. Pokud je IP adresa v seznamu bloků zásad (PBL), může vlastník přiřadit jinou statickou IP adresu nebo odebrat adresu z PBL.

- U blokovaných odchozích zpráv z vaší domény připojené k Microsoftu se tato chyba zobrazí, pokud jsou zprávy směrované přes službu třetí strany. Pomocí vyhledávacího nástroje WHOIS můžete najít blokovaného vlastníka IP adresy.
