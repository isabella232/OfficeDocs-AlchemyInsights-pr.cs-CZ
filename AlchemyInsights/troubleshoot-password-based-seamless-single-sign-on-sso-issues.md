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
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="99bc2-102">Řešení problémů s bezproblémovým jednotným přihlašováním (SSO) na základě hesla</span><span class="sxs-lookup"><span data-stu-id="99bc2-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="99bc2-103">Pokud se chcete dozvědět základní principy jednotného přihlašování založeného na heslech, přečtěte si informace o ověřování pomocí [hesla se službou Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="99bc2-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="99bc2-104">**Konfigurace jednotného přihlašování založeného na heslech**</span><span class="sxs-lookup"><span data-stu-id="99bc2-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="99bc2-105">[Konfigurace jednotného přihlašování založeného na heslech](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – tento článek obsahuje podrobnější informace o možnosti jednotného přihlašování založené na heslech.</span><span class="sxs-lookup"><span data-stu-id="99bc2-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="99bc2-106">Pokud aplikace, kterou přidáváte, vyžaduje vlastní konfiguraci a potřebujete použít jednotné přihlašování založené na heslem, je tento článek pro vás.</span><span class="sxs-lookup"><span data-stu-id="99bc2-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="99bc2-107">[Nakonfigurujte jednotné přihlašování na](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) základě hesla pro předchozí aplikace – proxy aplikace podporuje několik režimů jednotného přihlašování.</span><span class="sxs-lookup"><span data-stu-id="99bc2-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="99bc2-108">Přihlašování založené na hesly je určené pro aplikace, které k ověřování používají kombinaci uživatelského jména a hesla.</span><span class="sxs-lookup"><span data-stu-id="99bc2-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="99bc2-109">Když nakonfigurujete přihlašování pomocí hesla pro vaši aplikaci, musí se uživatelé přihlásit k místní aplikaci jednou.</span><span class="sxs-lookup"><span data-stu-id="99bc2-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="99bc2-110">Potom Azure Active Directory přihlašovací údaje uloží a automaticky je poskytne aplikaci, když se k ní uživatelé na dálku přistupují.</span><span class="sxs-lookup"><span data-stu-id="99bc2-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="99bc2-111">Už byste měli svou aplikaci publikovat a otestovat pomocí proxy serveru aplikace.</span><span class="sxs-lookup"><span data-stu-id="99bc2-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="99bc2-112">Pokud ne, postupujte podle pokynů v části Publikování aplikací pomocí proxy serveru aplikace [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a pak pokračujte v konfiguraci jednotného přihlašování založeného na hesly pro on-premové aplikace.</span><span class="sxs-lookup"><span data-stu-id="99bc2-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="99bc2-113">Pokud chcete řešit potíže s jednotným přihlašováním založeným na heslech, podívejte se na řešení potíží s jednotným přihlašováním založeným na hesle [v Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="99bc2-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
