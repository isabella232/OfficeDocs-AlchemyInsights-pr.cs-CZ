---
title: Řízení přístupu k veřejným složkám pomocí Outlooku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803516"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="52024-102">Řízení přístupu k veřejným složkám pomocí Outlooku</span><span class="sxs-lookup"><span data-stu-id="52024-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="52024-103">Řízení přístupu uživatelů k veřejným složkám v Outlooku:</span><span class="sxs-lookup"><span data-stu-id="52024-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="52024-104">Použití `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="52024-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="52024-105">$true: povolení přístupu uživatelů k veřejným složkám v Outlooku</span><span class="sxs-lookup"><span data-stu-id="52024-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="52024-106">$false: zabraňte přístupu uživatelů k veřejným složkám v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="52024-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="52024-107">Tato hodnota je výchozí.</span><span class="sxs-lookup"><span data-stu-id="52024-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="52024-108">Poznámka: Tento postup může řídit připojení pouze s desktopovou aplikací Outlook pro klienty Windows.</span><span class="sxs-lookup"><span data-stu-id="52024-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="52024-109">Uživatelé mohou dál přistupovat k veřejným složkám pomocí OWA nebo Outlooku for Mac.</span><span class="sxs-lookup"><span data-stu-id="52024-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="52024-110">Další informace najdete v tématu [řízená připojení k veřejným složkám v Outlooku](https://aka.ms/controlpf) , kde najdete další informace.</span><span class="sxs-lookup"><span data-stu-id="52024-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
