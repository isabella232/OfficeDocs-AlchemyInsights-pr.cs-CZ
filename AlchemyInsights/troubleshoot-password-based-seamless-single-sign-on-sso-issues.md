---
title: Řešení problémů s jednotným přihlašováním založeným na heslech
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972817"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Řešení problémů s jednotným přihlašováním založeným na heslech

Základní informace o jednotném přihlašování založeném na heslech najdete v tématu Ověřování založené na [heslech s Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurace jednotného přihlašování založeného na heslech**

1. [Konfigurace jednotného přihlašování založeného](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) na heslech – v tomto článku najdete další podrobnosti o možnosti jednotného přihlašování založeného na heslech. Pokud aplikace, kterou přidáváte, vyžaduje vlastní konfiguraci a potřebujete použít jednotné přihlašování založené na heslech, je tento článek pro vás.
2. [Konfigurace jednotného přihlašování založeného](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) na heslech pro předchozí aplikace – Proxy aplikace podporuje několik režimů jednotného přihlašování. Přihlašování založené na heslech je určené pro aplikace, které k ověřování používají kombinaci uživatelského jména a hesla. Když nakonfigurujete přihlašování pomocí hesla pro vaši aplikaci, musí se vaši uživatelé jednou přihlásit k místní aplikaci. Potom Azure Active Directory přihlašovací údaje a automaticky je poskytne aplikaci, když k ní budou mít uživatelé vzdálený přístup.
    - Aplikaci byste už měli publikovat a otestovat pomocí proxy serveru aplikace. Pokud ne, postupujte podle pokynů v článku Publikování aplikací pomocí Proxy aplikací [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a pak pokračujte v konfiguraci jednotného přihlašování založeného na heslech pro aplikace v počítači.

Řešení potíží s jednotným přihlašováním založeným na heslech najdete v tématu Poradce při potížích s jednotným přihlašováním založeným na [heslech v Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
