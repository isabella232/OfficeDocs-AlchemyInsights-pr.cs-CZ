---
title: Informace o identitě v Yammer
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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918930"
---
# <a name="about-identity-in-yammer"></a>Informace o identitě v Yammer

Doporučuje se, aby všechny sítě podnikané následující kroky, aby se předešlo problémům souvisejícím s identitou:

1. Vynucovat Office 365 identity po zřízení Microsoft 365 účtů pro uživatele ve službě Azure AD, abyste zajistili, že se všichni uživatelé přihlásí pomocí svého primárního Microsoft 365 účtu. Další informace najdete v tématu [Vynucení Office 365 identity Yammer uživatelů](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Sloučení více Yammer sítí. Starší Yammer umožňují připojení více Yammer sítí k jednomu tenantovi. Další informace najdete v tématu [Migrace sítě – sloučení více Yammer sítí](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Volitelně můžete vynucovat licencování Yammer, aby uživatelé Yammer uživatelům, pokud licenci nemají. Další informace najdete v tématu [Správa Yammer uživatelských licencí v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Nakonec můžete auditovat seznam uživatelů pro starší Yammer a pozastavit starší uživatele. Doporučujeme pozastavit (deaktivovat) uživatele místo jejich odstranění, protože odstranění je nevratné. Další informace najdete v tématu [Auditování Yammer v sítích připojených](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) k Office 365 [a Odebrání uživatelů](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Když nakonfigurujete Yammer tímto postupem, budete taky připravení nakonfigurovat síť Yammer pro nativní režim pro Microsoft 365. Další informace najdete v tématu Konfigurace [Yammer pro nativní režim pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).