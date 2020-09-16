---
title: Vytvoření webu v SharePointu Online
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
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732209"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="3a4d0-102">Vytvoření SharePointových webů pomocí šablon</span><span class="sxs-lookup"><span data-stu-id="3a4d0-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="3a4d0-103">Možnost Uložit web jako šablonu není pro moderní komunikaci ani týmové weby podporovaná.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="3a4d0-104">Další informace o používání šablon najdete v článku [uložení, stažení a nahrání sharepointového webu jako šablony](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="3a4d0-105">Tady jsou některé běžné problémy a řešení týkající se uložení webu nebo seznamu jako šablony v SharePointu Online.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="3a4d0-106">**Tlačítko Uložit šablonu webu/seznamu není k dispozici nebo chybí**</span><span class="sxs-lookup"><span data-stu-id="3a4d0-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="3a4d0-107">Aby bylo možné povolit funkce šablony, musí správci povolit vlastní skript.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3a4d0-108">Podrobné pokyny najdete v tématu Příklady a úvahy</span><span class="sxs-lookup"><span data-stu-id="3a4d0-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="3a4d0-109">Povolení nebo zakázání vlastního skriptu</span><span class="sxs-lookup"><span data-stu-id="3a4d0-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="3a4d0-110">Příkaz Uložit web jako šablonu není podporován a může způsobit problémy na webech, které používají infrastrukturu publikování serveru SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="3a4d0-111">**Šablonu webu nelze vytvořit nebo nefunguje správně**</span><span class="sxs-lookup"><span data-stu-id="3a4d0-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="3a4d0-112">V šabloně možná chybí [funkce](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje se.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="3a4d0-113">Pokud tuto funkci nelze aktivovat v aktuální kolekci webů, nelze k vytvoření webu použít šablonu webu.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="3a4d0-114">Zkontrolujte, jestli některé seznamy nebo knihovny nepřekročí [mezní hodnotu limit zobrazení seznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="3a4d0-115">Web pravděpodobně používá příliš mnoho zdrojů, a proto šablona webu překračuje limit 50 MB.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="3a4d0-116">Vyskytly se problémy se zobrazením dat ze seznamu, který používá vyhledávací sloupec.</span><span class="sxs-lookup"><span data-stu-id="3a4d0-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3a4d0-117">Další informace najdete v tématu [seznam vygenerovaný šablonou nezobrazuje data ze správného vyhledávacího seznamu v SharePointu Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="3a4d0-118">Podrobnější informace o běžných problémech a řešeních najdete v pro [vytváření a používání šablon webů](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3a4d0-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



