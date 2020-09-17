---
title: Došlo k chybě při ověřování tokenu přístupu v průběhu analýzy na ploše.
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783544"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="c64b2-102">Při prověřování desktopové analýzy došlo k chybě při ověřování tokenu přístupu</span><span class="sxs-lookup"><span data-stu-id="c64b2-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="c64b2-103">Tato chyba se obvykle zobrazuje, když vyprší platnost ověřovacího tokenu.</span><span class="sxs-lookup"><span data-stu-id="c64b2-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="c64b2-104">Obvykle se aktualizace stránky aktualizuje.</span><span class="sxs-lookup"><span data-stu-id="c64b2-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="c64b2-105">Tento problém ale může trvat i v případě, že jsou u účtu, který se používá k analýze desktopové analýzy, všechny zásady podmíněného přístupu.</span><span class="sxs-lookup"><span data-stu-id="c64b2-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="c64b2-106">V protokolech Azure AD se můžete podívat do protokolů v Azure Portalu a zjistit, jestli nedochází k chybám přihlašování pro účet, který se používá pro službu Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="c64b2-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="c64b2-107">Další informace o podmíněném přístupu najdete v tématu [Plánování nasazení podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="c64b2-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>