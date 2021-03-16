---
title: Řešení potíží s kódy chyb a zprávami jednotného přihlašování (SSO)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9367"
- "9004357"
ms.openlocfilehash: 805a85ffd47e14295c375fc415301570de22bfd8
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816095"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-error-codes-and-messages"></a><span data-ttu-id="ad433-102">Řešení potíží s kódy chyb a zprávami jednotného přihlašování (SSO)</span><span class="sxs-lookup"><span data-stu-id="ad433-102">Troubleshoot Seamless Single Sign-on (SSO) error codes and messages</span></span>

<span data-ttu-id="ad433-103">Pokud chcete vyřešit kódy chyb a zprávy jednotného přihlašování (SSO), postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="ad433-103">To resolve Seamless Single Sign-on (SSO) error codes and messages, perform the following steps:</span></span>

1. <span data-ttu-id="ad433-104">Zkontrolujte chyby jednotného přihlašování a vyřešte je tak, že se na portálu Azure Active Directory přihlásíte k sestavě aktivit [přihlášení.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)</span><span class="sxs-lookup"><span data-stu-id="ad433-104">Review and troubleshoot SSO errors by going to the [Sign-in activity reports in the Azure Active Directory portal](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins).</span></span>
2. <span data-ttu-id="ad433-105">Podívejte se na článek Řešení potíží s bezproblémovým jednotným přihlašováním k Azure [Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license) – tento článek vám pomůže najít informace o řešení běžných problémů týkajících se Azure Active Directory (Azure AD) Seamless Single Sign-On (Bezproblémové jednotné přihlašování).</span><span class="sxs-lookup"><span data-stu-id="ad433-105">See [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>
3. <span data-ttu-id="ad433-106">Podívejte [se na](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) článek Kódy chyb ověřování a autorizace Azure AD – tento článek vám pomůže najít informace o kódech chyb AADSTS, které se vrátily ze služby tokenů zabezpečení Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ad433-106">See [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) - This article helps you find information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS).</span></span> <span data-ttu-id="ad433-107">Tento článek vám taky pomůže najít popisy chyb AADSTS, opravy a některá navrhovaná alternativní řešení.</span><span class="sxs-lookup"><span data-stu-id="ad433-107">This article also helps you find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="ad433-108">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – Informace o vytváření žádostí o funkce nebo kladení technických otázek týkajících se bezproblémového jednotného přihlašování najdete v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="ad433-108">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - See this article for information on making feature requests or asking technical questions about Seamless SSO.</span></span>

