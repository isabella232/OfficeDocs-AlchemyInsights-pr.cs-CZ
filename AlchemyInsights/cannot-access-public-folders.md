---
title: Nelze získat přístup k veřejným složkám
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812540"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se nemůže připojit k veřejným složkám

Pokud pro některé uživatele nefunguje přístup ke veřejné složce, zkuste toto:

Připojte se k EXO PowerShellu a nakonfigurujte parametr DefaultPublicFolderMailbox na problémovém uživatelském účtu tak, aby odpovídal parametru na pracovním uživatelském účtu.

Pøíklad

Načíst – poštovní schránka WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Počkejte alespoň jednu hodinu, než se změna projeví.

Pokud problém potrvá [, postupujte podle](https://aka.ms/pfcte) pokynů k řešení problémů s přístupem k veřejným složkám pomocí Outlooku.
 
**Řízení přístupu uživatelů k veřejným složkám v Outlooku**:

1.  Use set-CASMailbox <mailboxname> -PublicFolderClientAccess $true nebo $false  
      
    $true: povolení přístupu uživatelů k veřejným složkám v Outlooku  
      
    $false: zabraňte přístupu uživatelů k veřejným složkám v Outlooku. Tato hodnota je výchozí.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Poznámka:** Tento postup může řídit připojení pouze s desktopovou aplikací Outlook pro klienty Windows. Uživatel může dál přistupovat k veřejným složkám v OWA nebo Outlooku pro Mac.
 
Další informace najdete v tématu [oznámení podpory řízeného připojení k veřejným složkám v Outlooku](https://aka.ms/controlpf).