---
title: Přidání externích uživatelů do distribuční skupiny
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934826"
---
# <a name="add-external-users-to-a-distribution-group"></a>Přidání externích uživatelů do distribuční skupiny

Přidání externího kontaktu do distribuční skupiny (DG) je dvoukrokový proces:
  
1. Vytvoření poštovního kontaktu pro externího uživatele:
    
    1. V Centru pro správu přejděte na **stránku Kontakty**  >  [uživatelů.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Vyberte **Přidat kontakt**.
    
    3. Zadejte informace o kontaktu a vyberte **Přidat**.
    
2. Přidejte e-mailový kontakt do svého GŘ:
    
    1. V Centru pro správu přejděte na stránku **Skupiny**  >  [](https://admin.microsoft.com/adminportal/home#/groups) skupin. 
    
    2. Najděte DG, ke které chcete přidat externího uživatele, a vyberte ho, abyste otevřeli dialogové okno pro úpravy.
    
    3. Na kartě **Členové** vyberte **Zobrazit všechny a spravovat členy**. 
    
    4. Vyberte **Přidat členy**.
    
    5. Vyberte poštovní kontakt, který jste vytvořili v předchozím kroku, a pak vyberte **Uložit**.
    
Pokud po provedení těchto kroků vaši externí uživatelé nesmějí posílat e-maily gř nebo z něj neobdrží e-maily, může to být tím, že je GŘ označené tak, aby povolo jenom e-maily od interních uživatelů. Tuto konfiguraci můžete zkontrolovat a opravit podle pokynů [tady](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Poznámka:** Tyto pokyny se nepoužijí, pokud je typ vaší skupiny "Microsoft 365" místo "Distribuční skupina". V takovém případě můžete externího uživatele přidat přímo do skupiny z Outlook. Podrobné informace o Microsoft 365 skupinách a pokyny pro přidání externích hostů najdete v [tomto článku.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  