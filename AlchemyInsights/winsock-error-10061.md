---
title: 1554 chyba Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698855"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="920f8-102">Chyba rozhraní Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="920f8-102">Winsock error 10061</span></span>

<span data-ttu-id="920f8-103">Tento chybový kód znamená, že Microsoft nemůže vytvořit soket TCP (připojení) s cílovým hostitelem.</span><span class="sxs-lookup"><span data-stu-id="920f8-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="920f8-104">Nejpravděpodobnější příčinou této chyby je problém s konfigurací brány firewall.</span><span class="sxs-lookup"><span data-stu-id="920f8-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="920f8-105">Tento problém můžete vyřešit kontrolou těchto nastavení:</span><span class="sxs-lookup"><span data-stu-id="920f8-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="920f8-106">Ověření konfigurace brány firewall informacemi v [adresách URL a IP adres Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="920f8-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="920f8-107">Pokud je chyba specifická pro Exchange Online Protection (EOP), měli byste se dřív upozornit na změnu [IP adres ochrany Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="920f8-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="920f8-108">Ověřte, že port neblokoval váš poskytovatel internetových služeb.</span><span class="sxs-lookup"><span data-stu-id="920f8-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="920f8-109">Ověřte nastavení inteligentního hostitele a cílového serveru ve svých konektorech.</span><span class="sxs-lookup"><span data-stu-id="920f8-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="920f8-110">Upozorňujeme, že Microsoft 365 tímto způsobem neblokuje *příchozí* připojení.</span><span class="sxs-lookup"><span data-stu-id="920f8-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
