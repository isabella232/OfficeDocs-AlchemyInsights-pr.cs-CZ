---
title: Project Online je ve stavu jen pro čtení.
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801645"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="51a2d-102">Project Online je ve stavu jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="51a2d-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="51a2d-103">Existují tři běžné důvody, proč Project Online může dosáhnout stavu jen pro čtení:</span><span class="sxs-lookup"><span data-stu-id="51a2d-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="51a2d-104">Organizace mají jenom licenci Projectu Online Essentials.</span><span class="sxs-lookup"><span data-stu-id="51a2d-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="51a2d-105">To si nestačí, aby byl web stále aktivní a nakonec se vám bude zobrazovat deaktivace.</span><span class="sxs-lookup"><span data-stu-id="51a2d-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="51a2d-106">Web můžete umístit do stavu jen pro čtení, aby správci věděli, že je to špatně a může získat správné licence.</span><span class="sxs-lookup"><span data-stu-id="51a2d-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="51a2d-107">Správci budou muset přidat Project Online Professional nebo Premium.</span><span class="sxs-lookup"><span data-stu-id="51a2d-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="51a2d-108">Web se v tomto bodě neobjeví jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="51a2d-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="51a2d-109">Další informace najdete v článku [porovnání řešení řízení projektů](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="51a2d-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="51a2d-110">Bylo dosaženo přidělené kvóty.</span><span class="sxs-lookup"><span data-stu-id="51a2d-110">Assigned quota has been reached.</span></span> <span data-ttu-id="51a2d-111">Další informace najdete v tématu [kvóty Project Web Appu](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="51a2d-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="51a2d-112">Pokud chcete zjistit, jak rozlišovací schopnost sestav ovlivňuje využití kvóty, zaškrtněte políčko [Konfigurovat souhrn časově uspořádaných dat sestav v Projectu Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) .</span><span class="sxs-lookup"><span data-stu-id="51a2d-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="51a2d-113">Jen pro čtení může být velmi dočasná podmínka, která se může během údržby vyskytnout.</span><span class="sxs-lookup"><span data-stu-id="51a2d-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="51a2d-114">Většina údržby ještě není pro naše zákazníky dokonce zajistěná a neuvidíte často tuto verzi, ale vyskytly se nějaké situace, kdy se vyskytly krátké doby.</span><span class="sxs-lookup"><span data-stu-id="51a2d-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
