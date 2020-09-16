---
title: Odstranění osamoceného uživatele z místního serveru
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
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680128"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Odstranění osamoceného uživatele z místního serveru

Pokud chcete odebrat osamoceného uživatele, postupujte takto:

1. Vynuťte synchronizaci adresářů podle pokynů v části [co je hybridní identita se službou Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Pokud chcete ověřit synchronizaci adresáře, podívejte se na téma [co je hybridní identita se službou Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Pokud funkce synchronizace správně funguje, ale odstranění objektu služby Active Directory se nešíří do služby Azure AD, odeberte osamocený objekt ručně pomocí jednoho z následujících rutin Azure Active Directory pro Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Pokud třeba chcete odebrat osamocený ID john.smith@contoso.com, které se původně vytvořilo pomocí synchronizace adresářů, spusťte tuto rutinu:

    Remove-MsolUser – UserPrincipalName John.Smith@Contoso.com