---
title: Dávka migrace veřejné složky se nedokončuje, zobrazuje se synchronizace.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803586"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="d3311-102">Dávka migrace veřejné složky se nedokončuje, zobrazuje se synchronizace.</span><span class="sxs-lookup"><span data-stu-id="d3311-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="d3311-103">Je možné, že jste zahájili dokončení dávky migrace a stav dávky migrace se velmi dlouho zobrazuje jako synchronizace.</span><span class="sxs-lookup"><span data-stu-id="d3311-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="d3311-104">Toto je očekávané chování.</span><span class="sxs-lookup"><span data-stu-id="d3311-104">This is expected behavior.</span></span>

<span data-ttu-id="d3311-105">Je běžné, že je stav dávky migrace ještě několik hodin, než se přepne na dokončení.</span><span class="sxs-lookup"><span data-stu-id="d3311-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="d3311-106">Pro migrace zahrnující velký počet cílových poštovních schránek je běžné, že se stav zobrazuje v synchronizovaném stavu déle než 24 hodin, pokud se žádný z uvedených požadavků na migraci veřejných složek nezdařil nebo nebyl umístěn do karantény.</span><span class="sxs-lookup"><span data-stu-id="d3311-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="d3311-107">Povolte 24-48 hodin pro dokončení úkolů dávky migrace.</span><span class="sxs-lookup"><span data-stu-id="d3311-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
