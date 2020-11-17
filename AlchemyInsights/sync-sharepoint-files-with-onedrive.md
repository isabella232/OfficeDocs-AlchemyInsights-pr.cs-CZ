---
title: Řešení potíží s příkazem „Otevřít v Průzkumníkovi“ v SharePointu Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086041"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="a8ec6-102">Řešení potíží s příkazem „Otevřít v Průzkumníkovi“ v SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="a8ec6-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="a8ec6-103">Postupujte podle kroků a doporučených postupů v následujících článcích:</span><span class="sxs-lookup"><span data-stu-id="a8ec6-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="a8ec6-104">Jak použít příkaz „Otevřít v Průzkumníkovi“ k řešení potíží v SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="a8ec6-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="a8ec6-105">Zkopírování nebo přesunutí souborů knihovny pomocí příkazu Otevřít v Průzkumníkovi</span><span class="sxs-lookup"><span data-stu-id="a8ec6-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="a8ec6-106">Doporučujeme [synchronizovat sharepointové soubory s novým synchronizačním klientem OneDrivu](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) , který poskytuje [soubory na vyžádání](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) , protože synchronizace uděluje místní přístup k vašim souborům a nabídne nejlepší výkon.</span><span class="sxs-lookup"><span data-stu-id="a8ec6-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="a8ec6-107">**Otevřít v Průzkumníkovi** je podporována jenom v Internet Exploreru 11.</span><span class="sxs-lookup"><span data-stu-id="a8ec6-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="a8ec6-108">Další informace najdete v článku [ukončení podpory pro IE11 s aplikacemi Microsoft 365](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy).</span><span class="sxs-lookup"><span data-stu-id="a8ec6-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="a8ec6-109">**Otevření v Průzkumníkovi** nefunguje v systému Windows s Microsoft Edgem, Google Chrome, Mozilla Firefox nebo na platformě Mac.</span><span class="sxs-lookup"><span data-stu-id="a8ec6-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="a8ec6-110">Z tohoto důvodu je možné možnost **zobrazení Průzkumníka zobrazit** šedě.</span><span class="sxs-lookup"><span data-stu-id="a8ec6-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="a8ec6-111">Tlačítko **Otevřít v Průzkumníkovi** se v novém prostředí knihovny nezobrazuje.</span><span class="sxs-lookup"><span data-stu-id="a8ec6-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="a8ec6-112">Vpravo nahoře vyberte z rozevíracího seznamu **Zobrazit** (jeho název se mění podle vašeho aktuálního zobrazení). Potom klikněte na **Zobrazit v Průzkumníkovi souborů**.</span><span class="sxs-lookup"><span data-stu-id="a8ec6-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

