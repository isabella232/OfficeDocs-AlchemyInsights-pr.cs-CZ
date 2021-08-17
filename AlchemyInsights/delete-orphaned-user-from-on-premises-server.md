---
title: Odstranění osiřelého uživatele z místního serveru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102237"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Odstranění osiřelého uživatele z místního serveru

Pokud chcete odebrat osiřelého uživatele, postupujte takto:

1. Vynucení synchronizace adresářů podle pokynů v tématu Co je hybridní identita s [Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Informace o ověření synchronizace adresářů najdete v tématu [Co je hybridní identita](https://technet.microsoft.com/library/jj151797.aspx)s Azure Active Directory? .

3. Pokud se synchronizační funkce správně nešíře do Azure AD, odeberte osamocené objekty ručně pomocí některé z následujících Azure Active Directory modulu pro Windows PowerShell rutin:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Pokud chcete například odebrat ID osamocené john.smith@contoso.com vytvořené pomocí synchronizace adresářů, spusťte rutinu:

    Remove-MsolUser – UserPrincipalName John.Smith@Contoso.com