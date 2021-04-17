---
title: Řízení přístupu k veřejným složkám pomocí Outlooku
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816733"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="b9403-102">Řízení přístupu k veřejným složkám pomocí Outlooku</span><span class="sxs-lookup"><span data-stu-id="b9403-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="b9403-103">Řízení přístupu uživatelů k veřejným složkám pomocí Outlooku:</span><span class="sxs-lookup"><span data-stu-id="b9403-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="b9403-104">Použití `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="b9403-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="b9403-105">$true: Povolení přístupu uživatelů k veřejným složkám v Outlooku</span><span class="sxs-lookup"><span data-stu-id="b9403-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="b9403-106">$false: Zabraňte přístupu uživatelů k veřejným složkám v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="b9403-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="b9403-107">Tato hodnota je výchozí.</span><span class="sxs-lookup"><span data-stu-id="b9403-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="b9403-108">Poznámka: Tento postup může řídit jenom připojení s desktopem Outlooku pro klienty s Windows.</span><span class="sxs-lookup"><span data-stu-id="b9403-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="b9403-109">Uživatelé mohou dál přistupovat k veřejným složkám pomocí aplikace OWA nebo Outlooku pro Mac.</span><span class="sxs-lookup"><span data-stu-id="b9403-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="b9403-110">Další informace najdete v tématu Řízená připojení k veřejným [složkám v Outlooku.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="b9403-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
