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
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813717"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Při odesílání e-mailu došlo k chybě: Hostitel klienta je zablokovaný pomocí spamhausu.

IP adresa, která zprávu odeslala, je v seznamu blokových bloků, který vlastní [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Mezi důvody, proč spamhaus blokuje, patří ohrožené účty, ohrožené počítače, které sdílejí veřejnou IP adresu, a zásady poskytovatele internetových služeb. Možné opravy jsou:
  
- U blokovaných příchozích zpráv, na kterých řídíte zdrojový e-mailový server, musíte určit příčinu a odebrat blok z webu Spamhaus.

- U blokovaných příchozích zpráv, u kterých zdrojová IP adresa patří někomu jinému, musí vlastník adresy odebrat blok z webu Spamhaus. Pokud je IP adresa v seznamu bloků zásad (PBL), může vlastník přiřadit jinou statickou IP adresu nebo odebrat adresu z PBL.

- U blokovaných odchozích zpráv z vaší domény připojené k Microsoftu se tato chyba zobrazí, pokud jsou zprávy směrované přes službu třetí strany. Pomocí vyhledávacího nástroje WHOIS můžete najít blokovaného vlastníka IP adresy.
