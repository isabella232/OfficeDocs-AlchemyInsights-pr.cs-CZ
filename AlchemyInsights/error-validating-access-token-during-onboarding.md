---
title: Při nástupu do desktopové analýzy došlo k chybě při ověřování přístupového tokenu.
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813681"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="f5faf-102">Chyba při ověřování přístupového tokenu při desktopové analýze</span><span class="sxs-lookup"><span data-stu-id="f5faf-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="f5faf-103">Tato chyba se obvykle pozoruje, když vyprší platnost ověřovacího tokenu.</span><span class="sxs-lookup"><span data-stu-id="f5faf-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="f5faf-104">Aktualizace stránky obvykle aktualizuje token.</span><span class="sxs-lookup"><span data-stu-id="f5faf-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="f5faf-105">Tento problém ale může přetrvávat, pokud existují nějaké zásady podmíněného přístupu použité u účtu používaného k místní desktopové analýze.</span><span class="sxs-lookup"><span data-stu-id="f5faf-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="f5faf-106">Na portálu Azure Portal si můžete zkontrolovat protokoly přihlášení k Azure AD a zjistit, jestli u účtu používaného pro přihlášení k desktopové analýze došlo k chybě přihlášení.</span><span class="sxs-lookup"><span data-stu-id="f5faf-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="f5faf-107">Další informace o podmíněném přístupu najdete na webu [Plánování nasazení podmíněného přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="f5faf-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>