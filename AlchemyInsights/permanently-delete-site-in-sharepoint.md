---
title: Trvalé odstranění webu v SharePointu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944304"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Trvalé odstranění webu v SharePointu

Pokud chcete znovu použít adresu URL z odstraněného webu (pro jeho opětovné vytvoření) nebo trvale odstranit web, protože už nepoužíváte, můžete využít funkci **trvalého odstranění** v novém Centru pro správu SharePointu. 

1. Přejděte na stránku [Odstraněné weby v novém Centru pro správu SharePointu](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) a přihlaste se pomocí účtu, který má pro vaši organizaci oprávnění správce. 

2. V levém sloupci vyberte web. 

3. Klikněte na **Trvale odstranit**. 

**Poznámka**: Weby spojené se skupinou se nedají z nového Centra pro správu SharePointu odstranit trvale. Místo toho bude potřeba použít [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Další informace najdete v článku [Trvalé odstranění webu](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
