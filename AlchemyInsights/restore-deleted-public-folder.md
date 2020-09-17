---
title: Obnovení odstraněné veřejné složky
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774524"
---
# <a name="restore-a-deleted-public-folder"></a>Obnovení odstraněné veřejné složky

**Obnovení odstraněných položek z veřejné složky**:

- [V outlooku 2016 se nedají obnovit odstraněné položky v nepoštovní veřejné složce](https://aka.ms/pfrec).
 
**Obnovení odstraněné veřejné složky (jakéhokoliv typu)**: 

- Použijte následující EXO PowerShellový příkaz:

    Syntaktická

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Příklad: následující příkaz obnoví Subfolder1 a umístí ho do \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Další informace najdete v článku [Obnovení odstraněné veřejné složky](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
