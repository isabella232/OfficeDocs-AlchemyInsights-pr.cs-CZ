---
title: Zásady pro hesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743441"
---
# <a name="password-policies"></a><span data-ttu-id="91e5c-102">Zásady pro hesla</span><span class="sxs-lookup"><span data-stu-id="91e5c-102">Password policies</span></span>

<span data-ttu-id="91e5c-103">**Mám problémy se zásadou hesla pro uživatele**</span><span class="sxs-lookup"><span data-stu-id="91e5c-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="91e5c-104">Zásady hesel pro uživatele závisí na tom, jestli je uživatel jenom v cloudu, nebo místně.</span><span class="sxs-lookup"><span data-stu-id="91e5c-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="91e5c-105">Jenom uživatelé v cloudu musí zvolit heslo, které splňuje požadavky uvedené v tomto článku: Zásady hesel, které se vztahují jenom [na cloudové uživatelské účty.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="91e5c-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="91e5c-106">Místní uživatelé musí zvolit heslo, které splňuje místní požadavky.</span><span class="sxs-lookup"><span data-stu-id="91e5c-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="91e5c-107">Pokud místní uživatel nemůže nastavit svoje heslo, zkontrolujte svoje místní požadavky.</span><span class="sxs-lookup"><span data-stu-id="91e5c-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="91e5c-108">**Nevím, jak nastavit nebo zkontrolovat zásady vypršení platnosti hesla**</span><span class="sxs-lookup"><span data-stu-id="91e5c-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="91e5c-109">Zásady vypršení platnosti pro cloudové uživatele v tenantovi můžete nastavit a zkontrolovat pomocí PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="91e5c-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="91e5c-110">Postupujte podle pokynů v tomto článku: Nastavení nebo kontrola [zásad hesel pomocí PowerShellu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="91e5c-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="91e5c-111">Zásady vypršení platnosti hesla pro místní uživatele jsou nastavené v místní službě AD.</span><span class="sxs-lookup"><span data-stu-id="91e5c-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="91e5c-112">**Další užitečné odkazy:**</span><span class="sxs-lookup"><span data-stu-id="91e5c-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="91e5c-113">Začínáme s resetováním hesla</span><span class="sxs-lookup"><span data-stu-id="91e5c-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="91e5c-114">Poradce při potížích s resetováním hesla iniciované správcem</span><span class="sxs-lookup"><span data-stu-id="91e5c-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
