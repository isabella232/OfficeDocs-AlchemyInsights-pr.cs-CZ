---
title: Problém se skupinami zabezpečení
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177386"
---
# <a name="issue-with-security-groups"></a>Problém se skupinami zabezpečení

**Pokud se zobrazí chyba sítě AADDS104**

Nejčastější příčinou chyb sítě pro Azure služba Active Directory Domain Services (služba AD DS) jsou neplatná pravidla skupiny zabezpečení služba AD DS. Skupina zabezpečení sítě pro virtuální síť musí povolit přístup ke konkrétním portům a protokolům. Pokud jsou tyto porty blokované, platforma Azure nemůže sledovat nebo aktualizovat spravovanou doménu. Má vliv také synchronizace mezi Azure AD a služba AD DS Azure. Zajistěte, abyste měli otevřené výchozí porty, abyste zabránili přerušení služby.

Informace o principech a řešení běžných upozornění týkajících se problémů s konfigurací skupiny zabezpečení sítě najdete v tématu [Přidání a ověření skupin zabezpečení.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
