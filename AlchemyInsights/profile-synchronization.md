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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kdy se synchronizace profilu změní do aplikace profilů uživatelů SharePointu?

SharePoint Online pomocí úlohy časovače importu služby Active Directory (import AD) umožňuje importovat uživatele a skupiny do aplikace profilů uživatelů. 
  
1. Import služby AD synchronizuje změny z úložiště adresářů SharePointu Online do aplikace profilů uživatelů. Tyto změny se zpracovávají v dávkách.
    
2. Úloha časovače se spustí, dokud se změny nesynchronizují.
    
> [!NOTE]
> Doba, po kterou bude úloha trvat, závisí na počtu změn procesu. Hodně změn trvá déle. Smlouva o úrovni služeb (SLA) uvádí, že se změna uživatele v adresáři SharePointu Online projeví v aplikaci profilů uživatelů za 24 hodin. 
  
[Další informace o synchronizaci profilů uživatelů v SharePointu Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

