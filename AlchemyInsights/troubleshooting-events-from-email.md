---
title: Řešení potíží s událostmi z e-mailu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834832"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="30a54-102">Řešení potíží s událostmi z e-mailu</span><span class="sxs-lookup"><span data-stu-id="30a54-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="30a54-103">Ověřte, jestli je pro poštovní schránku povolená funkce: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="30a54-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="30a54-104">Pak se podívejte na protokoly Události z **e-mailu Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="30a54-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="30a54-105">V protokolech Události z e-mailu najděte Id internetové zprávy, které odpovídá položce v poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="30a54-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="30a54-106">TrustScore určuje, jestli je položka přidaná nebo ne.</span><span class="sxs-lookup"><span data-stu-id="30a54-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="30a54-107">Události se přidávají jenom v případě, že trustscore = "Důvěryhodný".</span><span class="sxs-lookup"><span data-stu-id="30a54-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="30a54-108">TrustScore je určeno vlastnostmi SPF, Dkim nebo Dmarc, které jsou v záhlaví zprávy.</span><span class="sxs-lookup"><span data-stu-id="30a54-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="30a54-109">Zobrazení těchto vlastností:</span><span class="sxs-lookup"><span data-stu-id="30a54-109">To view these properties:</span></span>

<span data-ttu-id="30a54-110">**Desktopový Outlook**</span><span class="sxs-lookup"><span data-stu-id="30a54-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="30a54-111">Otevření položky</span><span class="sxs-lookup"><span data-stu-id="30a54-111">Open the item</span></span>
- <span data-ttu-id="30a54-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="30a54-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="30a54-113">nebo</span><span class="sxs-lookup"><span data-stu-id="30a54-113">or</span></span>

<span data-ttu-id="30a54-114">**KNIHOVNA MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="30a54-114">**MFCMapi**</span></span>

- <span data-ttu-id="30a54-115">Přechod na položku ve složce Doručená pošta</span><span class="sxs-lookup"><span data-stu-id="30a54-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="30a54-116">Hledejte PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="30a54-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="30a54-117">Tyto vlastnosti se určují a zaznamenávají během přenosu a směrování.</span><span class="sxs-lookup"><span data-stu-id="30a54-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="30a54-118">Pokud chcete další řešení potíží vyřešit, budete možná muset s podporou přenosu vyřešit chyby v SPF, DKIM a.nebo DMARC.</span><span class="sxs-lookup"><span data-stu-id="30a54-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>