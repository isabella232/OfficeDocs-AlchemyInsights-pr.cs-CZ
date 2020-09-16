---
title: Odstraňování potíží s událostmi z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658727"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="d0d64-102">Odstraňování potíží s událostmi z e-mailu</span><span class="sxs-lookup"><span data-stu-id="d0d64-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="d0d64-103">Ověřte, jestli je funkce pro poštovní schránku povolená: **Get- <mailbox> EventsFromEmailConfiguration-identity**</span><span class="sxs-lookup"><span data-stu-id="d0d64-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="d0d64-104">Potom se podívejte na události z e-mailu protokoly **exportovat – MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="d0d64-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="d0d64-105">V protokolech události z e-mailu Najděte InternetMessageId, který odpovídá položce v poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="d0d64-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="d0d64-106">TrustScore určuje, jestli je položka přidaná.</span><span class="sxs-lookup"><span data-stu-id="d0d64-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="d0d64-107">Události budou přidány pouze v případě, že je TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="d0d64-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="d0d64-108">TrustScore je určený vlastnostmi SPF, DKIM nebo DMARC, které jsou v záhlaví zprávy.</span><span class="sxs-lookup"><span data-stu-id="d0d64-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="d0d64-109">Zobrazení těchto vlastností:</span><span class="sxs-lookup"><span data-stu-id="d0d64-109">To view these properties:</span></span>

<span data-ttu-id="d0d64-110">**Desktopová aplikace Outlook**</span><span class="sxs-lookup"><span data-stu-id="d0d64-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="d0d64-111">Otevření položky</span><span class="sxs-lookup"><span data-stu-id="d0d64-111">Open the item</span></span>
- <span data-ttu-id="d0d64-112">Vlastnosti > souborů – > Internetová záhlaví</span><span class="sxs-lookup"><span data-stu-id="d0d64-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="d0d64-113">nebo</span><span class="sxs-lookup"><span data-stu-id="d0d64-113">or</span></span>

<span data-ttu-id="d0d64-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="d0d64-114">**MFCMapi**</span></span>

- <span data-ttu-id="d0d64-115">Přechod na položku ve složce Doručená pošta</span><span class="sxs-lookup"><span data-stu-id="d0d64-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="d0d64-116">Vyhledejte PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="d0d64-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="d0d64-117">Tyto vlastnosti se zjišťují a zaznamenávají při přenosu a směrování.</span><span class="sxs-lookup"><span data-stu-id="d0d64-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="d0d64-118">Pro další řešení potíží možná budete muset zpracovat podporu přenosu o chybách v SPF, DKIM a. nebo DMARC.</span><span class="sxs-lookup"><span data-stu-id="d0d64-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>