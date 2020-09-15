---
title: Starobní služby Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698675"
---
# <a name="access-services-retirement"></a><span data-ttu-id="a3052-102">Starobní služby Access Services</span><span class="sxs-lookup"><span data-stu-id="a3052-102">Access services retirement</span></span>

<span data-ttu-id="a3052-103">Jak jsme původně oznámili společnost Microsoft v MC97576, v březnu 2017 a pokračovali v komunikaci během minulého roku, jsou vyřazeny služby Access Services.</span><span class="sxs-lookup"><span data-stu-id="a3052-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="a3052-104">Další fází tohoto procesu bude odebrání webových databází Accessu, které používají seznamy SharePointu jako odpovídající úložiště dat.</span><span class="sxs-lookup"><span data-stu-id="a3052-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="a3052-105">**Jak se to týká?**</span><span class="sxs-lookup"><span data-stu-id="a3052-105">**How does this affect me?**</span></span>

<span data-ttu-id="a3052-106">Od června 2019 zastavíme vytváření nových Accessových databází v SharePointu Online a ukončete službu a všechny zbývající aplikace do dubna 2020.</span><span class="sxs-lookup"><span data-stu-id="a3052-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="a3052-107">**Co je potřeba udělat, abyste mohli připravit tuto změnu?**</span><span class="sxs-lookup"><span data-stu-id="a3052-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="a3052-108">Doporučujeme vytvořit plán přechodu pro webové databáze Accessu vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="a3052-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="a3052-109">Správci můžou pomocí [skeneru aplikace SharePoint pro Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) získat soupis aplikací pro Access, které weby používají.</span><span class="sxs-lookup"><span data-stu-id="a3052-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="a3052-110">Existuje několik způsobů migrace dat webových databází v Accessu:</span><span class="sxs-lookup"><span data-stu-id="a3052-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="a3052-111">Import do místní databáze Accessu (. ACCDB) nebo na excelový soubor.</span><span class="sxs-lookup"><span data-stu-id="a3052-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="a3052-112">Doporučujeme také prozkoumat Microsoft PowerApps jako alternativní platformu pro vytváření obchodních řešení pro webové a mobilní zařízení.</span><span class="sxs-lookup"><span data-stu-id="a3052-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>