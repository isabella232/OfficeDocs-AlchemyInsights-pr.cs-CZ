---
title: Aplikace pro ověřování
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404366"
---
# <a name="authentication-app"></a><span data-ttu-id="eb256-102">Aplikace pro ověřování</span><span class="sxs-lookup"><span data-stu-id="eb256-102">Authentication app</span></span>

<span data-ttu-id="eb256-103">Pokud jste globální správce, můžete rychle zjistit, co se stalo, nebo diagnostikovat problémy související s přihlášením uživatele pomocí [nástroje Diagnostika přihlášení](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="eb256-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="eb256-104">Spusťte diagnostiku kliknutím na tlačítko Spustit[diagnostiku.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="eb256-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="eb256-105">Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, čase přihlášení, ID žádosti nebo ID korelace.</span><span class="sxs-lookup"><span data-stu-id="eb256-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="eb256-106">Zkontrolujte diagnostické výsledky s podrobnostmi o tom, co se stalo, a jaké akce můžete provést, pokud jsou potřeba nějaké změny.</span><span class="sxs-lookup"><span data-stu-id="eb256-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="eb256-107">**Zkontrolujte scénář, který se použije:**</span><span class="sxs-lookup"><span data-stu-id="eb256-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="eb256-108">Pokud se uživateli v aplikaci Microsoft Authenticator nezobrazují nabízená oznámení, ověřte, že se nezobrazují pod blokovaným uživatelům MFA, jak je popsáno v článku Blokování a [odblokování uživatelů](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="eb256-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="eb256-109">Pokud uživatel není pro MFA zablokovaný, ale neobdrží nabízené oznámení, může otevřít aplikaci Microsoft Authenticator, která vyžádá čekající žádosti o schválení.</span><span class="sxs-lookup"><span data-stu-id="eb256-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="eb256-110">Jako alternativní způsob přihlášení může uživatel taky kliknout na Přihlásit se jiným způsobem a zvolit použití ověřovacího kódu z mobilní aplikace.</span><span class="sxs-lookup"><span data-stu-id="eb256-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="eb256-111">Aplikace Microsoft Authenticator je jedinou dostupnou metodou pro mnoho uživatelů.</span><span class="sxs-lookup"><span data-stu-id="eb256-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="eb256-112">[Přečtěte si další informace o výchozích](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)nastaveních zabezpečení , nejčastější dotazy k [aplikacím Authenticator,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) kde najdete nejčastější dotazy a jak je vyřešit.</span><span class="sxs-lookup"><span data-stu-id="eb256-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="eb256-113">**Doporučená videa**</span><span class="sxs-lookup"><span data-stu-id="eb256-113">**Recommended Videos**</span></span>

<span data-ttu-id="eb256-114">[Jak nastavit aplikaci Authenticator na novém telefonu (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="eb256-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
