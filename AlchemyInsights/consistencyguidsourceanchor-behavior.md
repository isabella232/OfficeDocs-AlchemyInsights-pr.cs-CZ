---
title: ConsistencyGuid / sourceAnchor behavior
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816985"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Connect (verze 1.1.524.0 a po) teď usnadňuje použití atributu msDS-ConsistencyGuid jako atributu sourceAnchor. Při použití této funkce Azure AD Connect automaticky nakonfiguruje pravidla synchronizace tak, aby:
  
- Jako atribut sourceAnchor pro objekty User použijte msDS-ConsistencyGuid. ObjectGUID se používá pro jiné typy objektů.
    
- U libovolného objektu místního uživatele služby AD, jehož atribut msDS-ConsistencyGuid není vyplněný, zapíše Azure AD Connect hodnotu svého objektuGUID zpátky do atributu msDS-ConsistencyGuid v místní službě Active Directory. Po naplnění atributu msDS-ConsistencyGuid exportuje Azure AD Connect objekt do Azure AD.
    
 **Poznámka:** Po importu místního objektu AD do Azure AD Connect (to znamená, že se importuje do prostoru konektoru AD a promítá se do metaverse), už nemůžete změnit jeho hodnotu sourceAnchor. Pokud chcete zadat hodnotu sourceAnchor pro daný místní objekt AD, nakonfigurujte jeho atribut msDS-ConsistencyGuid před importem do Azure AD Connect. 
  
Další informace o sourceanchoru a consistencyguidu najdete v následujících příkladech: [Azure AD Connect: Koncepty návrhu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

