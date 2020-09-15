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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663506"
---
# <a name="add-external-users-to-a-distribution-group"></a>Přidání externích uživatelů do distribuční skupiny

Přidání externího kontaktu do distribuční skupiny (DG) je proces se dvěma kroky:
  
1. Vytvoření e-mailového kontaktu pro externího uživatele:
    
    1. V centru pro správu přejděte na **Users**  >  stránku[Kontakty](https://admin.microsoft.com/adminportal/home#/Contact) pro uživatele. 
    
    2. Vyberte **Přidat kontakt**.
    
    3. Zadejte informace o kontaktu a vyberte **Přidat**.
    
2. Přidejte poštovní kontakt do svého DISTRIBUČNÍho systému:
    
    1. V centru pro správu přejděte na stránku skupiny **skupiny**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Najděte distribuční položku, ke které chcete externího uživatele přidat, a vyberte ji a otevřete tak dialogové okno Upravit.
    
    3. Na kartě **Členové** vyberte **Zobrazit všechny a spravovat členy**. 
    
    4. Vyberte **přidat členy**.
    
    5. Vyberte kontakt pošty, který jste vytvořili v předchozím kroku, a pak vyberte **Uložit**.
    
Pokud po provedení těchto kroků nebudou externí uživatelé moct posílat e-maily distribuční skupině nebo nedostávat e-maily, může to být, když je distribuční společnost označena tak, že povolí pouze e-maily od interních uživatelů. Můžete zkontrolovat tuto konfiguraci a opravit ji [podle pokynů.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Poznámka:** Tyto pokyny se nevztahují, pokud typ vaší skupiny je "skupina Microsoft 365" místo "distribuční skupina". V tom případě můžete externího uživatele přidat přímo do skupiny z Outlooku. Podrobné informace o skupinách společností Microsoft 365 a pokyny pro přidání externích hostů najdete v [tomto článku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  