---
title: Fond odchozích přenosů
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381596"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="73e8b-102">Fond odchozích přenosů</span><span class="sxs-lookup"><span data-stu-id="73e8b-102">Outbound relay pool</span></span>

<span data-ttu-id="73e8b-103">Microsoft v konfiguraci přenosu nebo přeposílání e-mailů prostřednictvím Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="73e8b-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="73e8b-104">Zprávy v určitých situacích se přeposílá nebo přeposílá přes Microsoft 365 pomocí speciálního fondu přenosů.</span><span class="sxs-lookup"><span data-stu-id="73e8b-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="73e8b-105">Zprávy odeslané pomocí fondu přenosů by mohly skončit ve složce nevyžádané pošty příjemce.</span><span class="sxs-lookup"><span data-stu-id="73e8b-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="73e8b-106">Další informace najdete v tématu [Fondy odchozích doručení.](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="73e8b-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="73e8b-107">Abyste se vyhnuli scénáři použití fondu přenosů, ujistěte se, že přeposlané/předáné zprávy splňují jedno z následujících kritérií:</span><span class="sxs-lookup"><span data-stu-id="73e8b-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="73e8b-108">Odchozí odesílatel je akceptována doména tenanta.</span><span class="sxs-lookup"><span data-stu-id="73e8b-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="73e8b-109">Rozhraní SPF (Sender Policy Framework) předá, když se zpráva zobrazí Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="73e8b-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="73e8b-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="73e8b-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="73e8b-111">Zprávy, které splňují výše uvedená kritéria, se přes fond přenosu nesměruje.</span><span class="sxs-lookup"><span data-stu-id="73e8b-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="73e8b-112">Pokud záznam MX pro vaši doménu odkazuje na server třetí strany nebo místního serveru, použijte vylepšené filtrování, abyste měli jistotu, že je ověření SPF správné pro příchozí e-maily a abyste se vyhnuli posílání e-mailů prostřednictvím fondu přenosu.</span><span class="sxs-lookup"><span data-stu-id="73e8b-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="73e8b-113">**Jak můžeme zjistit, jestli nás ovlivňuje fond přenosů?**</span><span class="sxs-lookup"><span data-stu-id="73e8b-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="73e8b-114">Pokud vaše přeposlané nebo předáené e-maily používají jedno z výše uvedených kritérií, zprávy se přes fond přenosů nepřesílat nebudou.</span><span class="sxs-lookup"><span data-stu-id="73e8b-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="73e8b-115">Pokud se ale zpráva odesílá prostřednictvím fondu přenosů, ip adresa odchozího serveru je v oblasti 40.95.0.0/16 a název odchozího serveru obsahuje **rly** v názvu.</span><span class="sxs-lookup"><span data-stu-id="73e8b-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

