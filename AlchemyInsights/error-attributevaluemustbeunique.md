---
title: Chyba AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709144"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AttributeValueMustBeUnique

Nejběžnějším důvodem pro chybu AttributeValueMustBeUnique jsou dva objekty, které mají v atributech ProxyAddresses a/nebo UserPrincipalName stejnou hodnotu. Oprava chyby AttributeValueMustBeUnique:
  
1. Identifikujte duplicitní proxyAddresses, userPrincipalName nebo jinou hodnotu atributu, která způsobuje chybu. Také určit, které dva (nebo více) objekty se do konfliktu účastní. Sestava generovaná stavem Azure AD Connect pro synchronizaci vám pomůže určit tyto dva objekty.
    
2. Určete, který objekt by měl dál mít duplicitní hodnotu a který objekt nemá.
    
3. Odebere duplicitní hodnotu z objektu, který tuto hodnotu nemá. Uvědomte si, že byste měli provést změnu v adresáři, ze kterého je objekt zdroj. V některých případech může být potřeba odstranit jeden z konfliktů.
    
4. Pokud jste provedli změnu v místních REKLAMách, umožněte službě Azure AD Connect změnu chyby, která se má opravit.
    

