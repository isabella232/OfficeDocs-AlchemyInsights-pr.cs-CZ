---
title: Jak povolit bezproblémové jednotné přihlašování
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825724"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="f94ea-102">Jak povolit bezproblémové jednotné přihlašování</span><span class="sxs-lookup"><span data-stu-id="f94ea-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="f94ea-103">Povolte bezproblémové jednotné přihlašování prostřednictvím [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="f94ea-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="f94ea-104">Pokud děláte novou instalaci Azure AD Connect, zvolte [vlastní instalační cestu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="f94ea-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="f94ea-105">Na **stránce Přihlášení uživatele** zvolte možnost Povolit **jednotné** přihlašování.</span><span class="sxs-lookup"><span data-stu-id="f94ea-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="f94ea-106">Pokud chcete ověřit, že jste bezproblémové jednotné přihlašování povolili správně:</span><span class="sxs-lookup"><span data-stu-id="f94ea-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="f94ea-107">Přihlaste se do Centra pro správu [Azure Active Directory](https://aad.portal.azure.com) jako globální správce.</span><span class="sxs-lookup"><span data-stu-id="f94ea-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="f94ea-108">V **levém podokně vyberte Azure Active Directory.**</span><span class="sxs-lookup"><span data-stu-id="f94ea-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="f94ea-109">Ověřte, jestli je možnost Bezproblémové jednotné **přihlašování povolená.**</span><span class="sxs-lookup"><span data-stu-id="f94ea-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="f94ea-110">Další informace najdete v tématu Bezproblémové jednotné přihlašování k [Azure Active Directory: Rychlý start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="f94ea-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  