---
title: Mapování knihovny SharePointu na síťovou jednotku
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 9115a3ab8d1234127a95628a9a49679ef06f6d39
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806176"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="1c55e-102">Mapování knihovny SharePointu na síťovou jednotku</span><span class="sxs-lookup"><span data-stu-id="1c55e-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="1c55e-103">Mapování knihovny jako síťové jednotky je dočasné a podporováno pouze prostřednictvím Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="1c55e-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="1c55e-104">V Internet Exploreru je třeba příležitostně otevřít web služby SharePoint a pak ukončit vypršení platnosti relace výběrem možnosti **zůstat přihlášení** .</span><span class="sxs-lookup"><span data-stu-id="1c55e-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="1c55e-105">Místo toho [synchronizujte soubory SharePointu s novým synchronizačním klientem OneDrivu](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) , </a> který poskytuje [soubory na vyžádání](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="1c55e-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="1c55e-106">Přístup ke všem souborům na OneDrivu bez použití prostoru místního úložiště</span><span class="sxs-lookup"><span data-stu-id="1c55e-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="1c55e-107">Pokud se místo [nového synchronizačního klienta OneDrivu](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)rozhodnete připojit jednotku, postupujte podle kroků uvedených v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="1c55e-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="1c55e-108">**Konfigurace a řešení potíží s mapovanými síťovými jednotkami**</span><span class="sxs-lookup"><span data-stu-id="1c55e-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="1c55e-109">Podívejte [se na Poradce při potížích s namapovanými síťovými jednotkami](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)</span><span class="sxs-lookup"><span data-stu-id="1c55e-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="1c55e-110">Poznámka: Pokud používáte Internet Explorer 10 s Windows 8 nebo Windows 7 a získáte **odepření přístupu** nebo když se při mapování jednotky **nezobrazuje cesta** , nainstalujte [tuto opravu hotfix](https://support.microsoft.com/help/2846960) , abyste tento problém vyřešili.</span><span class="sxs-lookup"><span data-stu-id="1c55e-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
