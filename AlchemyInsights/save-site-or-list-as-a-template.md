---
title: Uložení webu nebo seznamu jako šablony
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727524"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="0d34b-102">Uložení webu nebo seznamu jako šablony</span><span class="sxs-lookup"><span data-stu-id="0d34b-102">Save site or list as a template</span></span>

<span data-ttu-id="0d34b-103">Šablony webů služby SharePoint jsou předdefinované definice navržené pro konkrétní podnik.</span><span class="sxs-lookup"><span data-stu-id="0d34b-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="0d34b-104">Další informace najdete v tématu [použití šablon k vytvoření různých typů sharepointových webů](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="0d34b-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="0d34b-105">Tady jsou některé běžné problémy a řešení týkající se uložení webu nebo seznamu jako šablony v SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="0d34b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="0d34b-106">**Tlačítko Uložit šablonu webu nebo seznamu není k dispozici nebo chybí**.</span><span class="sxs-lookup"><span data-stu-id="0d34b-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="0d34b-107">Aby bylo možné povolit funkce šablony, musí správci povolit vlastní skript.</span><span class="sxs-lookup"><span data-stu-id="0d34b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="0d34b-108">Podrobné pokyny najdete v části [Povolení nebo zakázání vlastního skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="0d34b-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="0d34b-109">Příkaz Uložit web jako šablonu není podporován a může způsobit problémy na webech, které používají infrastrukturu publikování serveru SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="0d34b-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="0d34b-110">**Šablonu webu nelze vytvořit nebo nefunguje správně**</span><span class="sxs-lookup"><span data-stu-id="0d34b-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="0d34b-111">V šabloně možná chybí [funkce](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje se.</span><span class="sxs-lookup"><span data-stu-id="0d34b-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="0d34b-112">Pokud tuto funkci nelze aktivovat v aktuální kolekci webů, nelze k vytvoření webu použít šablonu webu.</span><span class="sxs-lookup"><span data-stu-id="0d34b-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="0d34b-113">Zkontrolujte, jestli některé seznamy nebo knihovny nepřekročí [mezní hodnotu limit zobrazení seznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000.</span><span class="sxs-lookup"><span data-stu-id="0d34b-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="0d34b-114">Web pravděpodobně používá příliš mnoho zdrojů, a proto šablona webu překračuje limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="0d34b-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="0d34b-115">Vyskytly se problémy se zobrazením dat ze seznamu, který používá vyhledávací sloupec.</span><span class="sxs-lookup"><span data-stu-id="0d34b-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="0d34b-116">Další informace najdete v tématu [seznam vygenerovaný šablonou nezobrazuje data ze správného vyhledávacího seznamu v SharePointu Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="0d34b-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="0d34b-117">Podrobnější informace o běžných problémech a řešeních najdete v informacích o [vytváření a používání šablon webů](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="0d34b-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

