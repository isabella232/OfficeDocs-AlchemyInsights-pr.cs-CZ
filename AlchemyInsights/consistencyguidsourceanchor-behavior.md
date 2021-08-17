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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044333"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor behavior

Azure AD Připojení (verze 1.1.524.0 a po) teď usnadňuje použití atributu msDS-ConsistencyGuid jako atributu sourceAnchor. Při použití této funkce Azure AD Připojení automaticky nakonfiguruje pravidla synchronizace tak, aby:
  
- Jako atribut sourceAnchor pro objekty User použijte msDS-ConsistencyGuid. ObjectGUID se používá pro jiné typy objektů.
    
- U libovolného objektu místního uživatele služby AD, jehož atribut msDS-ConsistencyGuid není vyplněný, zapíše Azure AD Připojení hodnotu svého objektuGUID zpátky do atributu msDS-ConsistencyGuid v místní službě Active Directory. Po naplnění atributu msDS-ConsistencyGuid azure AD Připojení objekt exportuje do Azure AD.
    
 **Poznámka:** Po importu místního objektu AD do Azure AD Připojení (to znamená, že se importuje do prostoru konektoru AD a promítá se do metaverse), už nemůžete změnit jeho hodnotu sourceAnchor. Pokud chcete zadat hodnotu sourceAnchor pro daný místní objekt AD, nakonfigurujte jeho atribut msDS-ConsistencyGuid před importem do azure AD Připojení. 
  
Další informace o sourceanchoru a consistencyguidu najdete v následujících příkladech: [Azure AD Připojení: Koncepty návrhu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

