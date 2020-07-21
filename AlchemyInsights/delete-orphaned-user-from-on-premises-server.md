---
title: Odstranění osamoceného uživatele z místního serveru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197939"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Odstranění osamoceného uživatele z místního serveru

Chcete-li odebrat osamoceného uživatele, postupujte takto:

1. Vynutit synchronizaci adresářů podle pokynů v části [Co je hybridní identita s Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)

2. Informace o ověření synchronizace adresářů naleznete v [tématu Co je hybridní identita s službou Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Pokud synchronizace funguje správně, ale odstranění objektu služby Active Directory se nerozšíří do služby Azure AD, ručně odeberte osamocený objekt pomocí jedné z následujících rutin modulu Azure Active Directory pro prostředí Windows PowerShell:

    Odstranit-MsolContact  
    Odebrat-MsolGroup  
    Odebrat-Msoluser

    Chcete-li například odebrat osamocené ID uživatele john.smith@contoso.com, původně vytvořené pomocí synchronizace adresářů, spusťte rutinu:

    Odebrat-MsolUser –UserPrincipalName John.Smith@Contoso.com