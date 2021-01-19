---
title: Chyby přihlášení uživatelů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900790"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="045a8-102">Chyby přihlášení uživatelů</span><span class="sxs-lookup"><span data-stu-id="045a8-102">User sign-in errors</span></span>

<span data-ttu-id="045a8-103">**Řešení problémů s diagnostickou pro přihlášení**</span><span class="sxs-lookup"><span data-stu-id="045a8-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="045a8-104">Pokud chcete zjistit příčinu nebo diagnostikovat problémy související s přihlašováním uživatelů, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="045a8-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="045a8-105">Spusťte diagnostický nástroj pro [přihlášení](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="045a8-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="045a8-106">Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, času přihlášení, ID žádosti nebo ID korelace.</span><span class="sxs-lookup"><span data-stu-id="045a8-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="045a8-107">Prohlédněte si výsledky diagnostických nástrojů s podrobnostmi o tom, co se stalo a jaké akce můžete provádět, pokud jsou potřeba.</span><span class="sxs-lookup"><span data-stu-id="045a8-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="045a8-108">**Hledáte informace o kódech chyb AADSTS, které jsou vraceny ze služby tokenů zabezpečení Azure Active Directory (STS)?**</span><span class="sxs-lookup"><span data-stu-id="045a8-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="045a8-109">V [tomto článku](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) najdete popis AADSTS chyb, opravy a některá navrhovaná řešení.</span><span class="sxs-lookup"><span data-stu-id="045a8-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>