---
title: Synchronizace profilů
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801762"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a7841-102">Kdy se synchronizace profilu změní do aplikace profilů uživatelů SharePointu?</span><span class="sxs-lookup"><span data-stu-id="a7841-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a7841-103">SharePoint Online pomocí úlohy časovače importu služby Active Directory (import AD) umožňuje importovat uživatele a skupiny do aplikace profilů uživatelů.</span><span class="sxs-lookup"><span data-stu-id="a7841-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a7841-104">Import služby AD synchronizuje změny z úložiště adresářů SharePointu Online do aplikace profilů uživatelů.</span><span class="sxs-lookup"><span data-stu-id="a7841-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a7841-105">Tyto změny se zpracovávají v dávkách.</span><span class="sxs-lookup"><span data-stu-id="a7841-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a7841-106">Úloha časovače se spustí, dokud se změny nesynchronizují.</span><span class="sxs-lookup"><span data-stu-id="a7841-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a7841-107">Doba, po kterou bude úloha trvat, závisí na počtu změn procesu.</span><span class="sxs-lookup"><span data-stu-id="a7841-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a7841-108">Hodně změn trvá déle.</span><span class="sxs-lookup"><span data-stu-id="a7841-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a7841-109">Smlouva o úrovni služeb (SLA) uvádí, že se změna uživatele v adresáři SharePointu Online projeví v aplikaci profilů uživatelů za 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="a7841-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a7841-110">Další informace o synchronizaci profilů uživatelů v SharePointu Online</span><span class="sxs-lookup"><span data-stu-id="a7841-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

