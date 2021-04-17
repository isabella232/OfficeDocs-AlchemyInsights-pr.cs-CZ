---
title: Události kalendáře chybí nebo se ne aktualizují
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837090"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="bc93b-102">Události kalendáře chybí nebo se ne aktualizují</span><span class="sxs-lookup"><span data-stu-id="bc93b-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="bc93b-103">Pokud položky kalendáře chybí nebo se ne aktualizují, začněte tím, že se podíváme na počet položek ve vlastnostech složky Kalendář v Outlooku:</span><span class="sxs-lookup"><span data-stu-id="bc93b-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="bc93b-104">Klikněte pravým tlačítkem myši na složku Kalendář **ovlivněného** uživatele a pak vyberte **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="bc93b-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="bc93b-105">Vyberte kartu **Synchronizace.**</span><span class="sxs-lookup"><span data-stu-id="bc93b-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="bc93b-106">Pokud počet položek není mezi složkami Server a Offline složka stejný:</span><span class="sxs-lookup"><span data-stu-id="bc93b-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="bc93b-107">**Zvýrazněte složku Kalendář.**</span><span class="sxs-lookup"><span data-stu-id="bc93b-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="bc93b-108">Přejděte na kartu **Odeslat** / **příjem** a pak vyberte **Aktualizovat složku**.</span><span class="sxs-lookup"><span data-stu-id="bc93b-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="bc93b-109">Pokud se kalendář pořád ne aktualizují nebo chybí události, stáhněte si Nástroj pro kontrolu kalendáře pro Outlook z [webu stažení Microsoftu.](https://www.microsoft.com/download/details.aspx?id=28786)</span><span class="sxs-lookup"><span data-stu-id="bc93b-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="bc93b-110">Zjistěte, jestli je ve složce kalendáře víc než 5 000 položek, protože to může způsobit příznaky, jako jsou například ne aktualizované schůzky kalendáře nebo chyby schůzky.</span><span class="sxs-lookup"><span data-stu-id="bc93b-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="bc93b-111">Další informace najdete v tématu Problémy s výkonem Outlooku, když je v souboru [.ost](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)nebo .pst v režimu mezipaměti příliš mnoho položek nebo složek.</span><span class="sxs-lookup"><span data-stu-id="bc93b-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>