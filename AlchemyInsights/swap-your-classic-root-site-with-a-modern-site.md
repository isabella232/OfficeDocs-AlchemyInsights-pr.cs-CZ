---
title: Výměna klasického kořenového webu s moderním webem
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691172"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="e40a5-102">Výměna klasického kořenového webu s moderním webem</span><span class="sxs-lookup"><span data-stu-id="e40a5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="e40a5-103">Pokud je vaše prostředí nastavené před duben 2019, můžete svůj kořenový web změnit na moderní web pomocí Microsoft PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="e40a5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="e40a5-104">Pokud máte jiný web, který chcete použít jako kořenový web, můžete [tento kořenový web nahradit (zaměňovat)](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="e40a5-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="e40a5-105">Pomocí metody [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zaměníte umístění webu s jiným webem při archivaci původního webu.</span><span class="sxs-lookup"><span data-stu-id="e40a5-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e40a5-106">K dispozici pro týmový web (nepřipojený ke skupině) a komunikační Web.</span><span class="sxs-lookup"><span data-stu-id="e40a5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="e40a5-107">Brzy budou zavedeny další možnosti, které vám umožní používat obsah na webu, ale převést existující web na komunikační Web.</span><span class="sxs-lookup"><span data-stu-id="e40a5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="e40a5-108">Tyto možnosti budou postupně shrnuty.</span><span class="sxs-lookup"><span data-stu-id="e40a5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="e40a5-109">Pokračujte v kontrole centra zpráv pro aktualizace.</span><span class="sxs-lookup"><span data-stu-id="e40a5-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e40a5-110">Známé problémy při záměně webů</span><span class="sxs-lookup"><span data-stu-id="e40a5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="e40a5-111">Cílový web může vrátit chybu "not found" (HTTP 404) po krátkou dobu.</span><span class="sxs-lookup"><span data-stu-id="e40a5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e40a5-112">Abyste mohli aktualizovat index vyhledávání, bude potřeba obsah znovu projít.</span><span class="sxs-lookup"><span data-stu-id="e40a5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e40a5-113">Není nutný žádný ruční krok – provede se to automaticky.</span><span class="sxs-lookup"><span data-stu-id="e40a5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="e40a5-114">Vše závislé na "statických" odkazech (například synchronizace souborů a soubory OneNotu) bude nutné ručně opravit.</span><span class="sxs-lookup"><span data-stu-id="e40a5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e40a5-115">Pokud byl zdrojový web webem organizace – příspěvky, aktualizujte adresu URL.</span><span class="sxs-lookup"><span data-stu-id="e40a5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="e40a5-116">Získejte seznam všech organizačních webů.</span><span class="sxs-lookup"><span data-stu-id="e40a5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="e40a5-117">Weby Project serveru bude pravděpodobně nutné ověřit, abyste se ujistili, že jsou pořád správně přidružené.</span><span class="sxs-lookup"><span data-stu-id="e40a5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
