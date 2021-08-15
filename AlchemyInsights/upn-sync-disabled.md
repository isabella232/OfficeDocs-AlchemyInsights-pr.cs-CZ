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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038105"
---
# <a name="upn-sync-disabled"></a>Synchronizace 4Dhod je zakázaná.

Pokud jste začali synchronizovat s Azure AD před 30. březnem 2016, spusťte následující rutinu Azure AD PowerShell, abyste povolovali soft match upn jenom pro vaši organizaci:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Automatická shoda upn se automaticky zapne pro organizace, které začaly synchronizovat s Azure AD 30. března 2016 nebo po tomto datu.
  
Další informace o povolení měkké shody s upn a dalšími funkcemi synchronizace najdete v tématu [Azure AD Připojení funkcí synchronizační služby](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

