---
title: Ve výsledcích hledání SharePointu se nezobrazuje obsah
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713123"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="c6623-102">Ve výsledcích hledání SharePointu se nezobrazuje obsah</span><span class="sxs-lookup"><span data-stu-id="c6623-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="c6623-103">Pokud se ve výsledcích hledání nezobrazuje očekávaný obsah, postupujte podle těchto kroků:</span><span class="sxs-lookup"><span data-stu-id="c6623-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="c6623-104">Zkontrolujte, jestli je **Web** obsahující očekávaný obsah nastavený tak, aby se obsah zobrazoval ve výsledcích hledání.</span><span class="sxs-lookup"><span data-stu-id="c6623-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="c6623-105">Postupujte podle pokynů v tématu [zobrazení obsahu na webu ve výsledcích hledání](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="c6623-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="c6623-106">Zkontrolujte, jestli je **seznam** nebo **Knihovna** obsahující očekávaný obsah nastavená tak, aby se obsah zobrazil ve výsledcích hledání.</span><span class="sxs-lookup"><span data-stu-id="c6623-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="c6623-107">Postupujte podle pokynů v tématu [zobrazení obsahu ze seznamů nebo knihoven ve výsledcích hledání](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="c6623-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="c6623-108">Ověřte, že je stránka, dokument nebo vlastní rozložení stránky publikované jako **hlavní verze.**</span><span class="sxs-lookup"><span data-stu-id="c6623-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="c6623-109">Postup při kroku 3 v [hledání nevrací všechny výsledky v SharePointu Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="c6623-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="c6623-110">Ověřte, jestli má uživatel **oprávnění** k zobrazení obsahu.</span><span class="sxs-lookup"><span data-stu-id="c6623-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="c6623-111">Postupujte podle pokynů v tématu [Principy úrovní oprávnění v SharePointu](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="c6623-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="c6623-112">Pokud se změnilo schéma vyhledávání přidáním nové spravované vlastnosti, upraví spravovanou vlastnost nebo odebráním spravované vlastnosti, která vyžaduje procházení a přeindexování.</span><span class="sxs-lookup"><span data-stu-id="c6623-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="c6623-113">**Znovu Indexujte** obsah podle pokynů v tématu [Ruční procházení a přeindexování webu, knihovny nebo seznamu](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="c6623-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="c6623-114">To může nějakou dobu trvat a až 24 hodin znovu zkontrolujte výsledky.</span><span class="sxs-lookup"><span data-stu-id="c6623-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="c6623-115">Další informace najdete v tématu [Povolení vyhledávání obsahu na webu](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="c6623-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
