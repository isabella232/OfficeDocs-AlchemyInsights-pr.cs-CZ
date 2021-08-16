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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002113"
---
# <a name="error-attributevaluemustbeunique"></a>Chyba: AttributeValueMustBeUnique

Nejběžnějším důvodem chyby AttributeValueMustBeUnique jsou dva objekty s různými objekty SourceAnchor (immutableId) mají stejnou hodnotu pro atributy ProxyAddresses nebo UserPrincipalName. Oprava chyby AttributeValueMustBeUnique:
  
1. Identifikujte duplicitní proxyAddresses, userPrincipalName nebo jinou hodnotu atributu, která způsobuje chybu. Také určete, které dva (nebo více) objektů jsou do konfliktu zapojeny. Sestava vygenerovaná službou Azure AD Připojení Stavu synchronizace vám může pomoct identifikovat dva objekty.
    
2. Určete, který objekt by měl mít duplicitní hodnotu a který objekt by neměl mít.
    
3. Odeberte duplicitní hodnotu z objektu, který by neměl mít hodnotu. Všimněte si, že byste měli udělat změnu v adresáři, ze které je objekt po zdroji. V některých případech může být potřeba odstranit některý z objektů, které jsou v konfliktu.
    
4. Pokud jste provedli změnu v místní službě AD, nechte Azure AD Připojení, aby se změna chyby opravili.
    

