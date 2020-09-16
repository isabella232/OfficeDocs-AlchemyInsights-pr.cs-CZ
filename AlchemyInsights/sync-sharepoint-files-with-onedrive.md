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
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737298"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b5502-102">Řešení potíží s příkazem „Otevřít v Průzkumníkovi“ v SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="b5502-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="b5502-103">Doporučujeme [synchronizovat sharepointové soubory přes nový synchronizační klient OneDrivu](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), který poskytuje [Soubory na požádání](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), protože zajišťuje místní přístup k souborům a nabízí nejlepší výkon.</span><span class="sxs-lookup"><span data-stu-id="b5502-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="b5502-104">Pokud chcete vyřešit problémy s funkcí Otevřít v Průzkumníkovi, postupujte podle kroků a osvědčených postupů v těchto článcích:</span><span class="sxs-lookup"><span data-stu-id="b5502-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="b5502-105">Jak použít příkaz „Otevřít v Průzkumníkovi“ k řešení potíží v SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="b5502-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="b5502-106">Zkopírování nebo přesunutí souborů knihovny pomocí příkazu Otevřít v Průzkumníkovi</span><span class="sxs-lookup"><span data-stu-id="b5502-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="b5502-107">**Poznámka:**</span><span class="sxs-lookup"><span data-stu-id="b5502-107">**Note:**</span></span>
>- <span data-ttu-id="b5502-108">Funkce Otevřít v Průzkumníkovi je podporovaná jenom v prohlížeči Internet Exploreru 10 nebo 11.</span><span class="sxs-lookup"><span data-stu-id="b5502-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b5502-109">Ve Windows příkaz Otevřít v Průzkumníkovi nefunguje v Microsoft Edgi, Google Chromu a Mozilla Firefoxu a nefunguje ani na platformě Mac.</span><span class="sxs-lookup"><span data-stu-id="b5502-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b5502-110">Proto může být volba Zobrazení Průzkumníka vyznačená šedě.</span><span class="sxs-lookup"><span data-stu-id="b5502-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="b5502-111">Tlačítko Otevřít v Průzkumníkovi se v novém prostředí knihovny nezobrazuje.</span><span class="sxs-lookup"><span data-stu-id="b5502-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b5502-112">Vpravo nahoře vyberte z rozevíracího seznamu **Zobrazit** (jeho název se mění podle vašeho aktuálního zobrazení). Potom klikněte na **Zobrazit v Průzkumníkovi souborů**.</span><span class="sxs-lookup"><span data-stu-id="b5502-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
