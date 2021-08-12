---
title: Obnovení odstraněné veřejné složky
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
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943368"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovení odstraněné veřejné složky

**Obnovení odstraněných položek z veřejné složky**:

- Další informace najdete v článku Odstraněné položky se neschová z veřejné složky, která není v [Outlook 2016.](https://aka.ms/pfrec)
 
**Obnovení odstraněné veřejné složky (libovolného typu):** 

- Použijte prosím následující příkaz EXO PowerShellu:

    Syntaxe:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Příklad: Následující příkaz obnoví podsložku1 a umístěte ji do složky \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Další podrobnosti najdete v článku Obnovení [odstraněné veřejné](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) složky.
