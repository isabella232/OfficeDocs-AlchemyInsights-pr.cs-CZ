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
# <a name="hide-public-folders"></a><span data-ttu-id="b5c06-102">Skrytí veřejných složek</span><span class="sxs-lookup"><span data-stu-id="b5c06-102">Hide public folders</span></span>

<span data-ttu-id="b5c06-103">**Skrytí celé stromové struktury veřejných složek:**</span><span class="sxs-lookup"><span data-stu-id="b5c06-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="b5c06-104">Pomocí postupu v [tomto článku můžete](https://aka.ms/ControlPF) u selektivně nebo u všech uživatelů skrýt celou stromovou strukturu veřejných složek.</span><span class="sxs-lookup"><span data-stu-id="b5c06-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="b5c06-105">**Skrytí konkrétní veřejné složky:**</span><span class="sxs-lookup"><span data-stu-id="b5c06-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="b5c06-106">Přidání oprávnění pro uživatele, kteří potřebují mít přístup k veřejné složce</span><span class="sxs-lookup"><span data-stu-id="b5c06-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="b5c06-107">Odeberte uživatele **Default** ze **seznamu** oprávnění:</span><span class="sxs-lookup"><span data-stu-id="b5c06-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
