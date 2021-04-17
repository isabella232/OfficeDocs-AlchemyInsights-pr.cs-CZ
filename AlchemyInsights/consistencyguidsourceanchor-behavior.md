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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="77b9e-102">ConsistencyGuid / sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="77b9e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="77b9e-103">Azure AD Connect (verze 1.1.524.0 a po) teď usnadňuje použití atributu msDS-ConsistencyGuid jako atributu sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="77b9e-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="77b9e-104">Při použití této funkce Azure AD Connect automaticky nakonfiguruje pravidla synchronizace tak, aby:</span><span class="sxs-lookup"><span data-stu-id="77b9e-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="77b9e-105">Jako atribut sourceAnchor pro objekty User použijte msDS-ConsistencyGuid.</span><span class="sxs-lookup"><span data-stu-id="77b9e-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="77b9e-106">ObjectGUID se používá pro jiné typy objektů.</span><span class="sxs-lookup"><span data-stu-id="77b9e-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="77b9e-107">U libovolného objektu místního uživatele služby AD, jehož atribut msDS-ConsistencyGuid není vyplněný, zapíše Azure AD Connect hodnotu svého objektuGUID zpátky do atributu msDS-ConsistencyGuid v místní službě Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77b9e-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="77b9e-108">Po naplnění atributu msDS-ConsistencyGuid exportuje Azure AD Connect objekt do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="77b9e-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="77b9e-109">**Poznámka:** Po importu místního objektu AD do Azure AD Connect (to znamená, že se importuje do prostoru konektoru AD a promítá se do metaverse), už nemůžete změnit jeho hodnotu sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="77b9e-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="77b9e-110">Pokud chcete zadat hodnotu sourceAnchor pro daný místní objekt AD, nakonfigurujte jeho atribut msDS-ConsistencyGuid před importem do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="77b9e-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="77b9e-111">Další informace o sourceanchoru a consistencyguidu najdete v následujících příkladech: [Azure AD Connect: Koncepty návrhu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="77b9e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

