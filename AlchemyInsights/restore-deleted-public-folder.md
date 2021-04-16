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
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809432"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovení odstraněné veřejné složky

**Obnovení odstraněných položek z veřejné složky**:

- Další informace najdete v článku Odstraněné položky v [Outlooku 2016](https://aka.ms/pfrec)se neschová z veřejné složky, která není poštovní.
 
**Obnovení odstraněné veřejné složky (libovolného typu):** 

- Použijte prosím následující příkaz EXO PowerShellu:

    Syntaxe:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Příklad: Následující příkaz obnoví podsložku1 a umístěte ji do složky \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Další podrobnosti najdete v článku Obnovení [odstraněné veřejné](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) složky.
