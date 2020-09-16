---
title: Blokování stahování v odkazech ke sdílení
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
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685735"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="1bfeb-102">Blokování stahování v odkazech ke sdílení</span><span class="sxs-lookup"><span data-stu-id="1bfeb-102">Block download on sharing links</span></span>

<span data-ttu-id="1bfeb-103">**Blokové stahování** je k dispozici **jen pro odkazy** na dokumenty Office.</span><span class="sxs-lookup"><span data-stu-id="1bfeb-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="1bfeb-104">Když vyberete tuto možnost, lidé, kteří získají přístup k souboru prostřednictvím vytvořeného odkazu, nebudou vidět možnosti pro stažení, tisk nebo kopírování souboru.</span><span class="sxs-lookup"><span data-stu-id="1bfeb-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="1bfeb-105">Správci můžou určit, jestli se má nastavení blokovat stahování zobrazovat jenom pro soubory Office, nebo změnit `BlockDownloadLinksFileType` nastavení v rutinách [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) nebo [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="1bfeb-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
