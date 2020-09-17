---
title: Nastavení DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808700"
---
# <a name="setup-dkim"></a>Nastavení DKIM

Kompletní pokyny ke konfiguraci DKIM pro vlastní domény v Microsoft 365 [najdete tady](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Pro **každou** vlastní doménu musíte vytvořit **dva** záznamy CNAME DKIM v hostitelské službě DNS vaší domény (obvykle doménového registrátora). Například contoso.com a fourthcoffee.com vyžadují čtyři DKIM záznamy CNAME: dvě pro contoso.com a dva pro fourthcoffee.com.

   Záznamy CNAME DKIM pro **každou** vlastní doménu používají následující formáty:

   - **Název hostitele**: `selector1._domainkey.<CustomDomain>`

     **Odkazuje na adresu nebo hodnotu**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Název hostitele**: `selector2._domainkey.<CustomDomain>`

     **Odkazuje na adresu nebo hodnotu**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je text nalevo od `.mail.protection.outlook.com` přizpůsobeného záznamu MX pro vlastní doménu (třeba `contoso-com` pro doménu contoso.com). \<InitialDomain\> je doména, kterou jste použili při registraci k Microsoft 365 (například contoso.onmicrosoft.com).

2. Po vytvoření záznamů CNAME pro vlastní domény postupujte takto:

   a. [Přihlaste se k Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocí svého pracovního nebo školního účtu.

   b. V levém horním rohu vyberte ikonu spouštěče aplikací a zvolte **Správce**.

   c. V navigačním panelu v levém dolním rohu rozbalte položku **správce** a zvolte **Exchange**.

   d. Přejděte na **Protection**  >  **DKIM**ochrany.

   e. Vyberte doménu a pak **pomocí DKIM podpisů pro tuto doménu**vyberte **Povolit** . Tento krok opakujte pro každou vlastní doménu.
