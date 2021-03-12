---
title: Tento web se neschová – chyba při pokusu o přístup k sharepointovém webu z prohlížeče nebo Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743438"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="e061a-102">Chyba "Tento web není možné dosáhnout" při pokusu o přístup k sharepointovém webu z prohlížeče nebo Teams</span><span class="sxs-lookup"><span data-stu-id="e061a-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="e061a-103">Uživatelé můžou při pokusu o přístup k sharepointovém webu z prohlížeče nebo Teams obdržet chybu "Tento web není možné dosáhnout".</span><span class="sxs-lookup"><span data-stu-id="e061a-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="e061a-104">Řešení tohoto problému:</span><span class="sxs-lookup"><span data-stu-id="e061a-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="e061a-105">Zkontrolujte, jestli je domovská stránka v koši nebo koši druhé fáze, a stránku obnovte.</span><span class="sxs-lookup"><span data-stu-id="e061a-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="e061a-106">**Ukázka přímé adresy URL do koše:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="e061a-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="e061a-107">Pokud je domovská stránka trvale odebrána z koše, vytvořte novou stránku webu z knihovny Stránky webu a vytvořte z ní domovskou stránku.</span><span class="sxs-lookup"><span data-stu-id="e061a-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="e061a-108">**Ukázková přímá adresa URL:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="e061a-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>