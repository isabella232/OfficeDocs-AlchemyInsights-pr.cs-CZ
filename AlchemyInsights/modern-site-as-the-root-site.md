---
title: Moderní web jako kořenový web
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666863"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="7d27a-102">Moderní web jako kořenový web</span><span class="sxs-lookup"><span data-stu-id="7d27a-102">Modern site as root site</span></span>

<span data-ttu-id="7d27a-103">Začali jsme vycházet s novou funkcí, která vám umožní [vyměnit kořenový web klasického webu pomocí moderního webu](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="7d27a-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="7d27a-104">Pomocí metody [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zaměníte umístění webu s jiným webem při archivaci původního webu.</span><span class="sxs-lookup"><span data-stu-id="7d27a-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="7d27a-105">K dispozici pro týmový web (nepřipojený ke skupině) a komunikační Web.</span><span class="sxs-lookup"><span data-stu-id="7d27a-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="7d27a-106">Neodstraňujte klasický kořenový web a vytvořte moderní komunikační Web.</span><span class="sxs-lookup"><span data-stu-id="7d27a-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="7d27a-107">Microsoft toto nepodporuje.</span><span class="sxs-lookup"><span data-stu-id="7d27a-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="7d27a-108">Když odstraníte kořenový web, budou všechny SharePointové weby ve vaší organizaci nedostupné všem uživatelům, dokud web neobnovíte nebo nevytvoříte nový web na stejné adrese URL.</span><span class="sxs-lookup"><span data-stu-id="7d27a-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="7d27a-109">Tuto funkci sdělujeme prostřednictvím centra zpráv.</span><span class="sxs-lookup"><span data-stu-id="7d27a-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="7d27a-110">Měli byste očekávat, že ve vašem klientovi brzy zapnete funkci.</span><span class="sxs-lookup"><span data-stu-id="7d27a-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="7d27a-111">Známé problémy při záměně webů</span><span class="sxs-lookup"><span data-stu-id="7d27a-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="7d27a-112">Cílový web může vrátit chybu "not found" (HTTP 404) po krátkou dobu.</span><span class="sxs-lookup"><span data-stu-id="7d27a-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="7d27a-113">Abyste mohli aktualizovat index vyhledávání, bude potřeba obsah znovu projít.</span><span class="sxs-lookup"><span data-stu-id="7d27a-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="7d27a-114">Zde není žádný ruční krok, který bude proveden automaticky.</span><span class="sxs-lookup"><span data-stu-id="7d27a-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="7d27a-115">Vše závislé na "statických" odkazech (například synchronizace souborů a soubory OneNotu) bude nutné ručně opravit.</span><span class="sxs-lookup"><span data-stu-id="7d27a-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="7d27a-116">Weby Project serveru bude pravděpodobně nutné ověřit, abyste se ujistili, že jsou pořád správně přidružené.</span><span class="sxs-lookup"><span data-stu-id="7d27a-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
