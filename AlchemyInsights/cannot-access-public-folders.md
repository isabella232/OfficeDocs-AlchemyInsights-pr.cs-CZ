---
title: Nelze získat přístup k veřejným složkám
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341396"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="57f5c-102">Outlook se nemůže připojit k veřejným složkám</span><span class="sxs-lookup"><span data-stu-id="57f5c-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="57f5c-103">Pokud pro některé uživatele nefunguje přístup ke veřejné složce, zkuste toto:</span><span class="sxs-lookup"><span data-stu-id="57f5c-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="57f5c-104">Připojte se k EXO PowerShellu a nakonfigurujte parametr DefaultPublicFolderMailbox na problémovém uživatelském účtu tak, aby odpovídal parametru na pracovním uživatelském účtu.</span><span class="sxs-lookup"><span data-stu-id="57f5c-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="57f5c-105">Pøíklad</span><span class="sxs-lookup"><span data-stu-id="57f5c-105">Example:</span></span>

<span data-ttu-id="57f5c-106">Načíst – poštovní schránka WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="57f5c-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="57f5c-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="57f5c-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="57f5c-108">Počkejte alespoň jednu hodinu, než se změna projeví.</span><span class="sxs-lookup"><span data-stu-id="57f5c-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="57f5c-109">Pokud problém potrvá [, postupujte podle](https://aka.ms/pfcte) pokynů k řešení problémů s přístupem k veřejným složkám pomocí Outlooku.</span><span class="sxs-lookup"><span data-stu-id="57f5c-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="57f5c-110">**Řízení přístupu uživatelů k veřejným složkám v Outlooku**:</span><span class="sxs-lookup"><span data-stu-id="57f5c-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="57f5c-111">Use set-CASMailbox <mailboxname> -PublicFolderClientAccess $true nebo $false</span><span class="sxs-lookup"><span data-stu-id="57f5c-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="57f5c-112">$true: povolení přístupu uživatelů k veřejným složkám v Outlooku</span><span class="sxs-lookup"><span data-stu-id="57f5c-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="57f5c-113">$false: zabraňte přístupu uživatelů k veřejným složkám v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="57f5c-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="57f5c-114">Tato hodnota je výchozí.</span><span class="sxs-lookup"><span data-stu-id="57f5c-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="57f5c-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="57f5c-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="57f5c-116">**Poznámka:** Tento postup může řídit připojení pouze s desktopovou aplikací Outlook pro klienty Windows.</span><span class="sxs-lookup"><span data-stu-id="57f5c-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="57f5c-117">Uživatel může dál přistupovat k veřejným složkám v OWA nebo Outlooku pro Mac.</span><span class="sxs-lookup"><span data-stu-id="57f5c-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="57f5c-118">Další informace najdete v tématu [oznámení podpory řízeného připojení k veřejným složkám v Outlooku](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="57f5c-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>