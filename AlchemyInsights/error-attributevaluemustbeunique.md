---
title: Chyba AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813753"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AttributeValueMustBeUnique

Nejběžnějším důvodem chyby AttributeValueMustBeUnique jsou dva objekty s různými objekty SourceAnchor (immutableId) mají stejnou hodnotu pro atributy ProxyAddresses nebo UserPrincipalName. Oprava chyby AttributeValueMustBeUnique:
  
1. Identifikujte duplicitní proxyAddresses, userPrincipalName nebo jinou hodnotu atributu, která způsobuje chybu. Také určete, které dva (nebo více) objektů jsou do konfliktu zapojeny. Sestava vygenerovaná službou Azure AD Connect Health pro synchronizaci vám může pomoct identifikovat dva objekty.
    
2. Určete, který objekt by měl mít duplicitní hodnotu a který objekt by neměl mít.
    
3. Odeberte duplicitní hodnotu z objektu, který by neměl mít hodnotu. Všimněte si, že byste měli udělat změnu v adresáři, ze které je objekt po zdroji. V některých případech může být potřeba odstranit některý z objektů, které jsou v konfliktu.
    
4. Pokud jste udělali změnu v místní službě AD, nechte Azure AD Connect synchronizovat změnu chyby, aby se opravili.
    

