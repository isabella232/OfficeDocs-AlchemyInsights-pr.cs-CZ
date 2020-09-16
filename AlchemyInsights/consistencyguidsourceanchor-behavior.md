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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b704e-102">Chování funkce ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="b704e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b704e-103">Azure AD Connect (verze 1.1.524.0 a After) teď usnadňuje použití atributu msDS-ConsistencyGuid as.</span><span class="sxs-lookup"><span data-stu-id="b704e-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b704e-104">Při použití této funkce Azure AD Connect automaticky konfiguruje synchronizační pravidla na:</span><span class="sxs-lookup"><span data-stu-id="b704e-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b704e-105">Jako atribut sourceAnchor objektů uživatelů použijte msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="b704e-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b704e-106">Objekt ObjectGUID se používá pro jiné typy objektů.</span><span class="sxs-lookup"><span data-stu-id="b704e-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b704e-107">V případě jakéhokoli daného místního uživatelského objektu služby Active Directory, jehož atribut msDS-ConsistencyGuid není naplněn, Azure AD Connect zapíše hodnotu objektu objectGUID zpátky na atribut msDS-ConsistencyGuid v místní službě Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b704e-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b704e-108">Po naplnění atributu msDS-ConsistencyGuid pak Azure AD Connect tento objekt exportuje do služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b704e-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b704e-109">**Poznámka:** Po naimportování místního objektu služby Active Directory do služby Azure AD Connect (to znamená, že je importován do prostoru připojovacího konektoru služby Active Directory a do úložiště metaverse) nelze změnit hodnotu sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="b704e-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b704e-110">Chcete-li zadat hodnotu sourceAnchor pro daný místní objekt Active Directory, nakonfigurujte před importem do služby Azure AD Connect jeho atribut msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="b704e-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b704e-111">Další informace o SourceAnchor a ConsistencyGuid najdete v těchto článcích: [Azure AD Connect: koncepce návrhů](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b704e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

