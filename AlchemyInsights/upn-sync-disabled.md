---
title: Synchronizace 4Dhod je zakázaná.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782144"
---
# <a name="upn-sync-disabled"></a>Synchronizace 4Dhod je zakázaná.

Pokud jste začali synchronizovat s Azure AD před 30. březnem 2016, spusťte následující rutinu Azure AD PowerShell, abyste povolovali soft match upn jenom pro vaši organizaci:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Automatická shoda upn se automaticky zapne pro organizace, které začaly synchronizovat s Azure AD 30. března 2016 nebo po tomto datu.
  
Další informace o povolení měkké shody v upn a dalších funkcích synchronizace najdete v tématu [Funkce synchronizační](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)služby Azure AD Connect .
  

