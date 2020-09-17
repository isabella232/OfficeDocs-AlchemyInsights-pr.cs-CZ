---
title: Jak povolit bezproblémové přihlašování k jednotnému přihlášení
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780520"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="aed21-102">Jak povolit bezproblémové přihlašování k jednotnému přihlášení</span><span class="sxs-lookup"><span data-stu-id="aed21-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="aed21-103">Povolte bezproblémové jednotné přihlašování prostřednictvím [služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="aed21-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="aed21-104">Pokud provádíte novou instalaci Azure AD Connect, zvolte [vlastní instalační cestu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="aed21-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="aed21-105">Na **přihlašovací stránce uživatele** zvolte možnost **Povolit jednotné přihlašování** .</span><span class="sxs-lookup"><span data-stu-id="aed21-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="aed21-106">Pokud chcete ověřit, jestli máte zapnuté bezproblémové jednotné přihlašování, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="aed21-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="aed21-107">Přihlaste se do [centra správy Azure Active Directory](https://aad.portal.azure.com) jako globální správce.</span><span class="sxs-lookup"><span data-stu-id="aed21-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="aed21-108">V levém podokně vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="aed21-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="aed21-109">Zkontrolujte, jestli je **povolené**bezproblémové jednotné přihlašování.</span><span class="sxs-lookup"><span data-stu-id="aed21-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="aed21-110">Další informace najdete v tématu [bezproblémové jednotné přihlašování v Azure Active Directory: rychlý Start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="aed21-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  