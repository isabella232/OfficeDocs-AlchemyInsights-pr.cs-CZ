---
title: Chování funkce ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756276"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Chování funkce ConsistencyGuid/sourceAnchor

Azure AD Connect (verze 1.1.524.0 a After) teď usnadňuje použití atributu msDS-ConsistencyGuid as. Při použití této funkce Azure AD Connect automaticky konfiguruje synchronizační pravidla na:
  
- Jako atribut sourceAnchor objektů uživatelů použijte msDS-ConsistencyGuid. Objekt ObjectGUID se používá pro jiné typy objektů.
    
- V případě jakéhokoli daného místního uživatelského objektu služby Active Directory, jehož atribut msDS-ConsistencyGuid není naplněn, Azure AD Connect zapíše hodnotu objektu objectGUID zpátky na atribut msDS-ConsistencyGuid v místní službě Active Directory. Po naplnění atributu msDS-ConsistencyGuid pak Azure AD Connect tento objekt exportuje do služby Azure AD.
    
 **Poznámka:** Po naimportování místního objektu služby Active Directory do služby Azure AD Connect (to znamená, že je importován do prostoru připojovacího konektoru služby Active Directory a do úložiště metaverse) nelze změnit hodnotu sourceAnchor. Chcete-li zadat hodnotu sourceAnchor pro daný místní objekt Active Directory, nakonfigurujte před importem do služby Azure AD Connect jeho atribut msDS-ConsistencyGuid. 
  
Další informace o SourceAnchor a ConsistencyGuid najdete v těchto článcích: [Azure AD Connect: koncepce návrhů](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

