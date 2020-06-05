---
title: Poradce při potížích s událostmi z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568940"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="a7d50-102">Poradce při potížích s událostmi z e-mailu</span><span class="sxs-lookup"><span data-stu-id="a7d50-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="a7d50-103">Ověřte, zda je funkce povolena pro poštovní schránku: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="a7d50-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="a7d50-104">Pak se podívejte na 'Události z e-mailu' protokoly **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="a7d50-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="a7d50-105">V protokolech Události z e-mailu najděte InternetMessageId, který odpovídá položce v poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="a7d50-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="a7d50-106">TrustScore určuje, zda je položka přidána nebo ne.</span><span class="sxs-lookup"><span data-stu-id="a7d50-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="a7d50-107">Události budou přidány pouze v případě, že TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="a7d50-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="a7d50-108">TrustScore je určena SPF, Dkim nebo Dmarc vlastnosti, které jsou v záhlaví zprávy.</span><span class="sxs-lookup"><span data-stu-id="a7d50-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="a7d50-109">Chcete-li zobrazit tyto vlastnosti:</span><span class="sxs-lookup"><span data-stu-id="a7d50-109">To view these properties:</span></span>

<span data-ttu-id="a7d50-110">**Outlook pro stolní počítače**</span><span class="sxs-lookup"><span data-stu-id="a7d50-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="a7d50-111">Otevření položky</span><span class="sxs-lookup"><span data-stu-id="a7d50-111">Open the item</span></span>
- <span data-ttu-id="a7d50-112">File -> Vlastnosti -> Internet Záhlaví</span><span class="sxs-lookup"><span data-stu-id="a7d50-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="a7d50-113">nebo</span><span class="sxs-lookup"><span data-stu-id="a7d50-113">or</span></span>

<span data-ttu-id="a7d50-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="a7d50-114">**MFCMapi**</span></span>

- <span data-ttu-id="a7d50-115">Přechod na položku v doručené poště</span><span class="sxs-lookup"><span data-stu-id="a7d50-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="a7d50-116">Podívejte se na PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="a7d50-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="a7d50-117">Tyto vlastnosti jsou určeny a zaznamenány během přenosu a směrování.</span><span class="sxs-lookup"><span data-stu-id="a7d50-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="a7d50-118">Pro další řešení potíží může být nutné sledovat s podporou přenosu o selhání v SPF, DKIM a.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="a7d50-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>