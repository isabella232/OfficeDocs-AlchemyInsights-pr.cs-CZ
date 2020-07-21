---
title: Uživatel obdrží chybu AADSTS7000112 Yammer je zakázán
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197793"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Uživatel obdrží chybu AADSTS7000112 Yammer je zakázán

Pokud se zobrazí chyba "AADSTS7000112: Aplikace '0000005-0000-0ff1-ce00-0000000000000'(Yammer) je zakázáno,, existuje problém s hlavním školitým v rámci služby Azure AD. Správce pravděpodobně zakázal objekt poskytování služeb, aby zablokoval přístup k Yammeru.

Zakázání objektu služby se nedoporučuje a může způsobit další problémy. Další informace o podporovaném přístupu k blokování přístupu uživatelů k Yammeru najdete v tématu [Vypnutí přístupu Yammeru pro uživatele Microsoftu 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Chcete-li tento problém opravit na webu Azure Portal a obnovit uživatelský přístup k Yammeru:

1.  Otevřete stránku Služby Active Directory Azure a v levém navigačním podokně vyberte **Možnost Spravovat** **podnikové aplikace.**
3.  Do vyhledávacího pole zadejte **Office 365 Yammer** a vyberte název aplikace, abyste otevřeli nastavení.
4.  V levém navigačním podokně vyberte **Vlastnosti** v části **Spravovat.**
5.  Nastavte hodnotu **Povoleno pro uživatele pro přihlášení?** na **Ano**a pak vyberte **Uložit**.
6.  Znovu se přihlaste k Yammeru. Možná budete muset vymazat soubory cookie.

Případně spusťte příkazy prostředí PowerShell a nastavte hodnotu. Další informace najdete [v tématu "Omlouváme se, ale máme potíže s přihlášením" při kliknutí na dlaždici Yammeru v Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 