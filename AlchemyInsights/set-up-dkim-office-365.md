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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108549"
---
# <a name="setup-dkim"></a>Nastavení DKIM

Kompletní pokyny pro konfiguraci DKIM pro vlastní domény v Microsoft 365 najdete [tady.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Pro **každou** vlastní doménu musíte vytvořit dva záznamy **CNAME** DKIM v hostitelské službě DNS vaší domény (obvykle doménového registrátora). Například contoso.com a fourthcoffee.com DKIM CNAME: dva pro contoso.com a dva pro fourthcoffee.com.

   Záznamy CNAME DKIM pro **každou** vlastní doménu používají následující formáty:

   - **Název hostitele:**`selector1._domainkey.<CustomDomain>`

     **Odkazuje na adresu nebo hodnotu:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Název hostitele:**`selector2._domainkey.<CustomDomain>`

     **Odkazuje na adresu nebo hodnotu:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> je text nalevo od přizpůsobeného záznamu MX pro vlastní doménu (například pro doménu `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>je doména, kterou jste použili při přihlášení k Microsoft 365 (například contoso.onmicrosoft.com).

2. Po vytvoření záznamů CNAME pro vlastní domény postupujte podle následujících pokynů:

   a. [přihlaste se Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pracovním nebo školním účtem.

   b. V levém horním rohu vyberte ikonu spouštěče aplikací a zvolte **Správce**.

   c. V levém dolním navigačním panelu rozbalte **Správce a** zvolte **Exchange**.

   d. Přejděte na **Ochrana**  >  **DKIM**.

   e. Vyberte doménu a pak zvolte **Povolit** pro podepisování **zpráv pro tuto doménu pomocí podpisů DKIM**. Tento krok opakujte pro každou vlastní doménu.
