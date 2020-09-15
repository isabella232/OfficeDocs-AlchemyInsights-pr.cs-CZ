---
title: Odepřený přístup při mapování jednotky na SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668736"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="bd7ca-102">Řešení problémů s knihovnami SharePoint mapovanými na síťové jednotky</span><span class="sxs-lookup"><span data-stu-id="bd7ca-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="bd7ca-103">Když přejdete na namapovanou síťovou jednotku, může se zobrazit jedna z těchto zpráv:</span><span class="sxs-lookup"><span data-stu-id="bd7ca-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="bd7ca-104">**\\Cesta není dostupná. Pravděpodobně nemáte oprávnění k používání tohoto síťového prostředku. Kontaktujte správce serveru a zjistěte, jestli máte přístupová oprávnění.**</span><span class="sxs-lookup"><span data-stu-id="bd7ca-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="bd7ca-105">**Přístup odepřen. Před otevřením souborů v tomto umístění musíte nejdřív přidat web do seznamu důvěryhodných webů, přejít na web a vybrat možnost automatického přihlašování.**</span><span class="sxs-lookup"><span data-stu-id="bd7ca-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="bd7ca-106">[Získejte pomoc s řešením potíží s mapovanými síťovými jednotkami](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="bd7ca-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="bd7ca-107">Mapování knihovny jako síťové jednotky je dočasné a podporováno pouze v Internet Exploreru.</span><span class="sxs-lookup"><span data-stu-id="bd7ca-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="bd7ca-108">Místo toho [synchronizujte sharepointové soubory pomocí nového synchronizačního klienta OneDrivu](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , který zahrnuje [soubory na vyžádání](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="bd7ca-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="bd7ca-109">Přístup ke všem souborům na OneDrivu bez použití prostoru místního úložiště</span><span class="sxs-lookup"><span data-stu-id="bd7ca-109">Access all your files in OneDrive without using local storage space.</span></span>
  