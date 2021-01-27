---
title: Problémy s podmíněným přístupem
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014746"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="13cea-102">Problémy s podmíněným přístupem</span><span class="sxs-lookup"><span data-stu-id="13cea-102">Conditional access issues</span></span>

<span data-ttu-id="13cea-103">**Řešení problémů s diagnostickou pro přihlášení**</span><span class="sxs-lookup"><span data-stu-id="13cea-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="13cea-104">Pomocí [diagnostických nástrojů pro přihlášení](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)můžete rychle zjistit, co se stalo nebo jak diagnostikovat problémy související s přihlašováním:</span><span class="sxs-lookup"><span data-stu-id="13cea-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="13cea-105">Spusťte diagnostický nástroj pro přihlášení.</span><span class="sxs-lookup"><span data-stu-id="13cea-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="13cea-106">Najděte událost, kterou chcete analyzovat, zadáním informací o uživateli, aplikaci, času přihlášení, ID žádosti nebo ID korelace.</span><span class="sxs-lookup"><span data-stu-id="13cea-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="13cea-107">Prohlédněte si výsledky diagnostických nástrojů s podrobnostmi o tom, co se stalo a jaké akce můžete provést, abyste udělali změny (pokud jsou potřeba nějaké změny).</span><span class="sxs-lookup"><span data-stu-id="13cea-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="13cea-108">**Řešení potíží s přihlášením**</span><span class="sxs-lookup"><span data-stu-id="13cea-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="13cea-109">Přejděte na přihlašovací stránku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13cea-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="13cea-110">Filtrovat přihlášení podle uživatele, časového rozsahu, aplikace, stavu, klientské aplikace atd.</span><span class="sxs-lookup"><span data-stu-id="13cea-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="13cea-111">Vyberte přihlašovací událost a zobrazte kartu pro podmíněný přístup a zjistěte, které zásady byly vyhodnoceny.</span><span class="sxs-lookup"><span data-stu-id="13cea-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="13cea-112">Kliknutím na řádek zásad zobrazte podrobnosti o zásadách a zjistěte, proč to byla použita.</span><span class="sxs-lookup"><span data-stu-id="13cea-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="13cea-113">**Nástroje pro řešení potíží s zásadou podmíněného přístupu**</span><span class="sxs-lookup"><span data-stu-id="13cea-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="13cea-114">Režim pouze sestavy umožňuje vyhodnotit zásady bez ovlivnění uživatelů.</span><span class="sxs-lookup"><span data-stu-id="13cea-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="13cea-115">Nástroj citlivosti umožňuje simulovat události přihlášení a zjistit, které zásady se používají.</span><span class="sxs-lookup"><span data-stu-id="13cea-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="13cea-116">V sešitě přehledů a sestav se zobrazuje dopad jednotlivých zásad v reálném čase.</span><span class="sxs-lookup"><span data-stu-id="13cea-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="13cea-117">**Zásady ochrany základní úrovně**</span><span class="sxs-lookup"><span data-stu-id="13cea-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="13cea-118">Zásady ochrany podle směrného plánu byly zastaralé.</span><span class="sxs-lookup"><span data-stu-id="13cea-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="13cea-119">Už se nevynucují a brzy se odeberou z Azure Portalu.</span><span class="sxs-lookup"><span data-stu-id="13cea-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="13cea-120">Doporučujeme povolit [výchozí nastavení zabezpečení](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="13cea-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="13cea-121">Další informace o podmíněném přístupu najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="13cea-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="13cea-122">[Osvědčené postupy pro podmíněný přístup v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Podmínky v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ovládací prvky v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Umístění v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="13cea-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
