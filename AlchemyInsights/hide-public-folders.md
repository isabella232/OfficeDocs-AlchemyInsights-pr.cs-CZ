---
title: Skrytí veřejných složek
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315337"
---
# <a name="hide-public-folders"></a>Skrytí veřejných složek

**Skrytí celé stromové struktury veřejných složek:**

Pomocí postupu v [tomto článku můžete](https://aka.ms/ControlPF) u selektivně nebo u všech uživatelů skrýt celou stromovou strukturu veřejných složek.

**Skrytí konkrétní veřejné složky:**

1. Přidání oprávnění pro uživatele, kteří potřebují mít přístup k veřejné složce

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Odeberte uživatele **Default** ze **seznamu** oprávnění:

    `Remove-PublicFolderClientPermission \test1 -User Default`
