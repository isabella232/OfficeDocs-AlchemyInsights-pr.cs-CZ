---
title: Problémy s připojením k SharePoint designeru
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
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727164"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="843af-102">Problémy s připojením k SharePoint designeru</span><span class="sxs-lookup"><span data-stu-id="843af-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="843af-103">Pokud v aplikaci SharePoint Designer dochází k problémům s připojením k webům SharePoint, vyzkoušejte následující běžná řešení.</span><span class="sxs-lookup"><span data-stu-id="843af-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="843af-104">Krok 1: Ověřte, jestli je SharePoint Designer 2013 aktualizovaný pomocí [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [aktualizace 2016 pro SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="843af-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="843af-105">Krok 2: vymazání souborů místní mezipaměti:</span><span class="sxs-lookup"><span data-stu-id="843af-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="843af-106">Zavřete SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="843af-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="843af-107">V místním počítači odeberte všechny soubory nalezené ve všech následujících složkách.</span><span class="sxs-lookup"><span data-stu-id="843af-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="843af-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="843af-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="843af-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="843af-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="843af-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="843af-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="843af-111">Otevřete SharePoint Designer 2013 a znovu zadejte účet, abyste viděli, jestli funguje.</span><span class="sxs-lookup"><span data-stu-id="843af-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="843af-112">Krok 3: [Povolte moderní ověřování pro Office 2013 na zařízeních s Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="843af-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="843af-113">Krok 4: Správci budou muset povolit připojení k SharePoint designeru pomocí **vlastního skriptu** v nastavení centra pro správu SharePointu.</span><span class="sxs-lookup"><span data-stu-id="843af-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="843af-114">Další informace najdete v tématu [Povolení nebo zakázání vlastního skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="843af-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


