---
title: O identitě v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148199"
---
# <a name="about-identity-in-yammer"></a>O identitě v Yammeru

Doporučuje se, aby všechny sítě provést následující kroky, aby se zabránilo problémy související s identitou:

1. Vynuťte identitu Office 365 po zřizování účtů Microsoft 365 pro uživatele ve službě Azure AD, abyste zajistili, že se všichni uživatelé přihlásí pomocí svého primárního účtu Microsoft 365. Další informace najdete v [tématu Vynucení identity Office 365 pro uživatele Yammeru](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidujte více sítí Yammer. Starší konfigurace Yammeru umožňují připojení více sítí Yammeru k jednomu klientovi. Další informace najdete v [tématu Migrace v síti – konsolidace více sítí Yammeru](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Volitelně můžete vynutit licencování pro Yammer, aby uživatelé z Yammeru zablokovali, pokud nemají licenci. Další informace najdete [v tématu Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Nakonec auditovat seznam uživatelů pro starší sítě Yammer a pozastavit starší uživatele. Doporučujeme uživatele pozastavit (deaktivovat) namísto jejich odstranění, protože odstranění je nevratné. Další informace najdete v [tématech Auditování uživatelů Yammeru v sítích připojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [Odebrání uživatelů](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Pokud yammer nakonfigurujete pomocí těchto kroků, budete taky připraveni nakonfigurovat síť Yammeru pro nativní režim pro Microsoft 365. Další informace najdete v [tématu Konfigurace sítě Yammer pro nativní režim pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).