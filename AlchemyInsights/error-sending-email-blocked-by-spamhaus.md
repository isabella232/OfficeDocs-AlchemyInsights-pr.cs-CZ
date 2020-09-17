---
title: Chyba při posílání e-mailů blokovaných uživatelem SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783796"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Chyba při odesílání e-mailů: hostitel klienta zablokovaný pomocí Spamhaus

IP adresa, která zprávu odeslala, je ve vlastnictví seznamu blokovaných [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Důvody zablokování uživatelem Spamhaus zahrnují ohrožení účtů, ohrožené počítače sdílející veřejnou IP adresu a zásady poskytovatele internetových služeb. Možné opravy:
  
- Pokud chcete blokovat příchozí zprávy, kde se řídí zdrojový e-mailový server, musíte určit příčinu a odebrat blok z webu spamhaus.

- Pro blokované příchozí zprávy, kde zdrojová IP adresa patří někomu jinému, musí vlastník adresy odebrat blok z webu spamhaus. Pokud je adresa IP v seznamu blok zásad (PBL), vlastník může přiřadit jinou statickou IP adresu nebo odebrat adresu z PBL.

- Pokud chcete blokovat odchozí zprávy z vaší domény připojené k Microsoftu, může se zobrazit tato chybová zpráva, pokud jsou zprávy směrovány přes službu třetích stran. K vyhledání vlastníka blokované IP adresy můžete použít vyhledávací nástroj WHOIS.
