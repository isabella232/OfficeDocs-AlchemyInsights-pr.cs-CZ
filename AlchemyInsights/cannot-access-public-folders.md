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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996623"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se nemůže připojit k veřejným složkám

Pokud přístup k veřejné složce některým uživatelům nefunguje, zkuste toto:

Připojení exo PowerShellu a nakonfigurujte parametr DefaultPublicFolderMailbox na problémový uživatelský účet tak, aby odpovídal parametru v pracovním uživatelském účtu.

Příklad:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Počkejte aspoň jednu hodinu, než se změna projeví.

Pokud problém přetrvává, [vyřešte](https://aka.ms/pfcte) prosím pomocí tohoto postupu problémy s přístupem k veřejné složce pomocí Outlook.
 
**Řízení přístupu uživatelů k veřejným složkám pomocí Outlook:**

1.  Použití Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true nebo $false  
      
    $true: Povolení přístupu uživatelů k veřejným složkám v Outlook  
      
    $false: Zabraňte přístupu uživatelů k veřejným složkám v Outlook. Tato hodnota je výchozí.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Poznámka:** Tento postup může řídit připojení jenom u Outlook plochy pro Windows klienty. Uživatel může dál přistupovat k veřejným složkám pomocí aplikace OWA nebo Outlook pro Mac.
 
Další informace najdete v článku Oznámení podpory řízených připojení k veřejným složkám [v Outlook](https://aka.ms/controlpf).