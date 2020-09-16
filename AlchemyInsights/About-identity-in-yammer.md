---
title: O identitě v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664163"
---
# <a name="about-identity-in-yammer"></a>O identitě v Yammeru

Doporučujeme, aby všechny sítě vybraly následující kroky, aby nedošlo k problémům s identitou:

1. Po zřízení účtů Microsoft 365 pro uživatele v Azure AD vynuťte identitu Office 365, aby se všichni uživatelé přihlásili pomocí svého primárního účtu Microsoft 365. Další informace najdete v článku [vynucení identity Office 365 pro uživatele Yammeru](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidujte více sítí Yammer. Starší konfigurace Yammeru umožňují spojení více sítí Yammer s jedním nájemcem. Další informace najdete v tématu [migrace sítě – sloučení více sítí Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Volitelně můžete vynucením licencování pro Yammer blokovat uživatele z Yammeru, pokud nemají licenci. Další informace najdete v článku [Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Nakonec zkontrolujte seznam uživatelů pro starší sítě Yammer a pozastavte starší uživatele. Doporučujeme, abyste uživatelé přezastavili (deaktivoval), protože odstranění je nevratné. Další informace najdete v článku [auditování uživatelů Yammeru v sítích připojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [odebrání uživatelů](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfigurací Yammeru pomocí těchto kroků budete moct taky nakonfigurovat svou síť Yammer pro nativní režim pro Microsoft 365. Další informace najdete v článku [Konfigurace sítě Yammer pro nativní režim pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).