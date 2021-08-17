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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320702"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kdy se změny profilu synchronizují s aplikací SharePoint profilu uživatele?

SharePoint Online používá úlohu časovače importu služby Active Directory (import ad) k importu uživatelů a skupin do aplikace profilů uživatelů. 
  
1. Import služby AD synchronizuje změny z SharePoint Online Directory Store do aplikace profilů uživatelů. Tyto změny se zpracovávají v dávkách.
    
2. Úloha časovače se spustí, dokud se změny nesynchronují.
    
**Poznámka:** Doba, kterou trvá spuštění úlohy, závisí na počtu změn, které se budou zpracovávat. Velký počet změn trvá déle. Smlouva SLA (Service Level Agreement) uvádí, že změna uživatele v adresáři SharePoint Online se projeví v aplikaci Profil uživatele za 24 hodin. 
  
[Další informace o synchronizaci profilu uživatele v SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

