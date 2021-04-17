---
title: Nelze získat přístup k veřejným složkám.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819505"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="6842a-102">Outlook se nemůže připojit k veřejným složkám</span><span class="sxs-lookup"><span data-stu-id="6842a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="6842a-103">Pokud přístup k veřejné složce některým uživatelům nefunguje, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="6842a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="6842a-104">Připojte se k EXO PowerShellu a nakonfigurujte parametr DefaultPublicFolderMailbox na problémový uživatelský účet tak, aby odpovídal parametru na pracovním uživatelském účtu.</span><span class="sxs-lookup"><span data-stu-id="6842a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="6842a-105">Příklad:</span><span class="sxs-lookup"><span data-stu-id="6842a-105">Example:</span></span>

<span data-ttu-id="6842a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="6842a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="6842a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="6842a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="6842a-108">Počkejte aspoň jednu hodinu, než se změna projeví.</span><span class="sxs-lookup"><span data-stu-id="6842a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="6842a-109">Pokud problém přetrvává, vyřešte prosím pomocí [tohoto](https://aka.ms/pfcte) postupu problémy s přístupem k veřejné složce v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="6842a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="6842a-110">**Řízení přístupu uživatelů k veřejným složkám pomocí Outlooku:**</span><span class="sxs-lookup"><span data-stu-id="6842a-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="6842a-111">Použití Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true nebo $false</span><span class="sxs-lookup"><span data-stu-id="6842a-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="6842a-112">$true: Povolení přístupu uživatelů k veřejným složkám v Outlooku</span><span class="sxs-lookup"><span data-stu-id="6842a-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="6842a-113">$false: Zabraňte přístupu uživatelů k veřejným složkám v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="6842a-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="6842a-114">Tato hodnota je výchozí.</span><span class="sxs-lookup"><span data-stu-id="6842a-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="6842a-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="6842a-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="6842a-116">**Poznámka:** Tento postup může řídit připojení jenom s desktopem Outlooku pro klienty s Windows.</span><span class="sxs-lookup"><span data-stu-id="6842a-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="6842a-117">Uživatel může dál přistupovat k veřejným složkám pomocí OWA nebo Outlooku pro Mac.</span><span class="sxs-lookup"><span data-stu-id="6842a-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="6842a-118">Další informace najdete v článku Oznámení podpory řízených připojení k veřejným [složkám v Outlooku](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="6842a-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>