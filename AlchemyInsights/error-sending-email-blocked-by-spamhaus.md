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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="41232-102">Při odesílání e-mailu došlo k chybě: Hostitel klienta je zablokovaný pomocí spamhausu.</span><span class="sxs-lookup"><span data-stu-id="41232-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="41232-103">IP adresa, která zprávu odeslala, je v seznamu blokových bloků, který vlastní [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="41232-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="41232-104">Mezi důvody, proč spamhaus blokuje, patří ohrožené účty, ohrožené počítače, které sdílejí veřejnou IP adresu, a zásady poskytovatele internetových služeb.</span><span class="sxs-lookup"><span data-stu-id="41232-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="41232-105">Možné opravy jsou:</span><span class="sxs-lookup"><span data-stu-id="41232-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="41232-106">U blokovaných příchozích zpráv, na kterých řídíte zdrojový e-mailový server, musíte určit příčinu a odebrat blok z webu Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="41232-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="41232-107">U blokovaných příchozích zpráv, u kterých zdrojová IP adresa patří někomu jinému, musí vlastník adresy odebrat blok z webu Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="41232-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="41232-108">Pokud je IP adresa v seznamu bloků zásad (PBL), může vlastník přiřadit jinou statickou IP adresu nebo odebrat adresu z PBL.</span><span class="sxs-lookup"><span data-stu-id="41232-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="41232-109">U blokovaných odchozích zpráv z vaší domény připojené k Microsoftu se tato chyba zobrazí, pokud jsou zprávy směrované přes službu třetí strany.</span><span class="sxs-lookup"><span data-stu-id="41232-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="41232-110">Pomocí vyhledávacího nástroje WHOIS můžete najít blokovaného vlastníka IP adresy.</span><span class="sxs-lookup"><span data-stu-id="41232-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
