---
title: Mapování atributů pro zřizování uživatelů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949666"
---
# <a name="user-provisioning-attribute-mapping"></a>Mapování atributů pro zřizování uživatelů

1. Informace o řešení známých problémů s mapováním atributů najdete v tématu [mapování atributů](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) poskytuje podporu pro zřizování uživatelů pro aplikace SaaS třetích stran, jako jsou Salesforce, G Suite a další. Pokud povolíte zřizování uživatelů pro aplikaci SaaS pro třetí strany, portál Azure ho řídí jeho hodnoty atributů prostřednictvím mapování atributů. Informace o tom, jak přizpůsobit výchozí mapování atributů, najdete v tématu [přizpůsobení atributu zřizování uživatelů – mapování pro aplikace SaaS v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Další informace o zřizování uživatelů aplikace pro SaaS najdete v tématu [co je automatizované zřizování aplikací aplikace SaaS v Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Při přizpůsobení mapování atributů pro zřizování uživatelů se může stát, že se atribut, který chcete mapovat, nezobrazí v seznamu zdrojových atributů. [Synchronizace atributu z vaší místní služby Active Directory do služby Azure AD pro zřizování](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) v článku aplikace vám ukáže, jak přidat chybějící atribut tím, že ho synchronizuje z vaší místní služby AD s Azure AD.
