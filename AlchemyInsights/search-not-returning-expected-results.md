---
title: 1491 – hledání – nevracení – očekávané – výsledky
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740467"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="978b1-102">Hledání obsahu nevrací očekávané výsledky</span><span class="sxs-lookup"><span data-stu-id="978b1-102">Content Search not returning expected results</span></span>

<span data-ttu-id="978b1-103">Když spouštíte hledání obsahu z centra zabezpečení Microsoft 365 Security &, může se zobrazit neočekávané výsledky hledání.</span><span class="sxs-lookup"><span data-stu-id="978b1-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="978b1-104">Zvažte následující věci, které můžou mít vliv na výsledky hledání:</span><span class="sxs-lookup"><span data-stu-id="978b1-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="978b1-105">**Umístění obsahu a podmínky vyhledávání**: Ujistěte se, že jste vybrali správná umístění obsahu a podmínky vyhledávání.</span><span class="sxs-lookup"><span data-stu-id="978b1-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="978b1-106">Pokud jste spustili velké vyhledávání (s mnoha umístěními), zvažte možnost rozdělení do několika hledání.</span><span class="sxs-lookup"><span data-stu-id="978b1-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="978b1-107">**Částečně indexované položky**:  [částečně indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštovních schránek se zahrnují do odhadovaných výsledků hledání.</span><span class="sxs-lookup"><span data-stu-id="978b1-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="978b1-108">Částečně indexované položky z webů v SharePointu a OneDrivu se ale do odhadu hledání nezahrnují.</span><span class="sxs-lookup"><span data-stu-id="978b1-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="978b1-109">**Neúspěšné hledání**: při hledání velkého počtu poštovních schránek (přes 100 000 poštovních schránek) se můžou zobrazit chyby hledání pomocí kódů chyb, jako je CS008-009 a CS012-002).</span><span class="sxs-lookup"><span data-stu-id="978b1-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="978b1-110">V tomto případě opakujte hledání pouze pro umístění s neúspěšným obsahem.</span><span class="sxs-lookup"><span data-stu-id="978b1-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="978b1-111">Další informace najdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="978b1-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
