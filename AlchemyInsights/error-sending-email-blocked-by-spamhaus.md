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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="ae39d-102">Chyba při odesílání e-mailů: hostitel klienta zablokovaný pomocí Spamhaus</span><span class="sxs-lookup"><span data-stu-id="ae39d-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="ae39d-103">IP adresa, která zprávu odeslala, je ve vlastnictví seznamu blokovaných [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="ae39d-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="ae39d-104">Důvody zablokování uživatelem Spamhaus zahrnují ohrožení účtů, ohrožené počítače sdílející veřejnou IP adresu a zásady poskytovatele internetových služeb.</span><span class="sxs-lookup"><span data-stu-id="ae39d-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="ae39d-105">Možné opravy:</span><span class="sxs-lookup"><span data-stu-id="ae39d-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="ae39d-106">Pokud chcete blokovat příchozí zprávy, kde se řídí zdrojový e-mailový server, musíte určit příčinu a odebrat blok z webu spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ae39d-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="ae39d-107">Pro blokované příchozí zprávy, kde zdrojová IP adresa patří někomu jinému, musí vlastník adresy odebrat blok z webu spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ae39d-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="ae39d-108">Pokud je adresa IP v seznamu blok zásad (PBL), vlastník může přiřadit jinou statickou IP adresu nebo odebrat adresu z PBL.</span><span class="sxs-lookup"><span data-stu-id="ae39d-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="ae39d-109">Pokud chcete blokovat odchozí zprávy z vaší domény připojené k Microsoftu, může se zobrazit tato chybová zpráva, pokud jsou zprávy směrovány přes službu třetích stran.</span><span class="sxs-lookup"><span data-stu-id="ae39d-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="ae39d-110">K vyhledání vlastníka blokované IP adresy můžete použít vyhledávací nástroj WHOIS.</span><span class="sxs-lookup"><span data-stu-id="ae39d-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
