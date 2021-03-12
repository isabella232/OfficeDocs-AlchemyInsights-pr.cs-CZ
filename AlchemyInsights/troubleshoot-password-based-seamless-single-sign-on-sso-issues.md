---
title: Řešení problémů s bezproblémovým jednotným přihlašováním (SSO) na základě hesla
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714708"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Řešení problémů s bezproblémovým jednotným přihlašováním (SSO) na základě hesla

Pokud se chcete dozvědět základní principy jednotného přihlašování založeného na heslech, přečtěte si informace o ověřování pomocí [hesla se službou Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurace jednotného přihlašování založeného na heslech**

1. [Konfigurace jednotného přihlašování založeného na heslech](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – tento článek obsahuje podrobnější informace o možnosti jednotného přihlašování založené na heslech. Pokud aplikace, kterou přidáváte, vyžaduje vlastní konfiguraci a potřebujete použít jednotné přihlašování založené na heslem, je tento článek pro vás.
2. [Nakonfigurujte jednotné přihlašování na](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) základě hesla pro předchozí aplikace – proxy aplikace podporuje několik režimů jednotného přihlašování. Přihlašování založené na hesly je určené pro aplikace, které k ověřování používají kombinaci uživatelského jména a hesla. Když nakonfigurujete přihlašování pomocí hesla pro vaši aplikaci, musí se uživatelé přihlásit k místní aplikaci jednou. Potom Azure Active Directory přihlašovací údaje uloží a automaticky je poskytne aplikaci, když se k ní uživatelé na dálku přistupují.
    - Už byste měli svou aplikaci publikovat a otestovat pomocí proxy serveru aplikace. Pokud ne, postupujte podle pokynů v části Publikování aplikací pomocí proxy serveru aplikace [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a pak pokračujte v konfiguraci jednotného přihlašování založeného na hesly pro on-premové aplikace.

Pokud chcete řešit potíže s jednotným přihlašováním založeným na heslech, podívejte se na řešení potíží s jednotným přihlašováním založeným na hesle [v Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
