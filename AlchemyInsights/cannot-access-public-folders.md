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
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se nemůže připojit k veřejným složkám

Pokud přístup k veřejné složce některým uživatelům nefunguje, zkuste toto:

Připojte se k EXO PowerShellu a nakonfigurujte parametr DefaultPublicFolderMailbox na problémový uživatelský účet tak, aby odpovídal parametru na pracovním uživatelském účtu.

Příklad:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Počkejte aspoň jednu hodinu, než se změna projeví.

Pokud problém přetrvává, vyřešte prosím pomocí [tohoto](https://aka.ms/pfcte) postupu problémy s přístupem k veřejné složce v Outlooku.
 
**Řízení přístupu uživatelů k veřejným složkám pomocí Outlooku:**

1.  Použití Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true nebo $false  
      
    $true: Povolení přístupu uživatelů k veřejným složkám v Outlooku  
      
    $false: Zabraňte přístupu uživatelů k veřejným složkám v Outlooku. Tato hodnota je výchozí.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Poznámka:** Tento postup může řídit připojení jenom s desktopem Outlooku pro klienty s Windows. Uživatel může dál přistupovat k veřejným složkám pomocí OWA nebo Outlooku pro Mac.
 
Další informace najdete v článku Oznámení podpory řízených připojení k veřejným [složkám v Outlooku](https://aka.ms/controlpf).