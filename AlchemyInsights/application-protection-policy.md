---
title: Zásady ochrany aplikací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423430"
---
# <a name="application-protection-policy"></a><span data-ttu-id="b7d0c-102">Zásady ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="b7d0c-102">Application protection policy</span></span>

<span data-ttu-id="b7d0c-103">Pokud se zásadami ochrany aplikací (APP) začínáte, podívejte se na [přehled zásad ochrany aplikací](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="b7d0c-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="b7d0c-104">Pokud chcete začít používat aplikaci APP, přečtěte [si téma Jak vytvořit a přiřadit zásady ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="b7d0c-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="b7d0c-105">Požadavky zásad ochrany aplikací:</span><span class="sxs-lookup"><span data-stu-id="b7d0c-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="b7d0c-106">Uživatel má licenci Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="b7d0c-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="b7d0c-107">Uživatel patří do skupiny, na kterou se zaměřují zásady ochrany aplikací.</span><span class="sxs-lookup"><span data-stu-id="b7d0c-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="b7d0c-108">K chráněným aplikacím na zařízení je přihlášen pouze jeden podnikový uživatel.</span><span class="sxs-lookup"><span data-stu-id="b7d0c-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="b7d0c-109">Aplikace implementovala [intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="b7d0c-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="b7d0c-110">Seznam aplikací, které sadu SDK podporují, najdete v tématu [Chráněné aplikace Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="b7d0c-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="b7d0c-111">Zásady platí poté, co se uživatel, který splňuje výše uvedené požadavky, přihlásí do aplikace s povolenou intune SDK.</span><span class="sxs-lookup"><span data-stu-id="b7d0c-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="b7d0c-112">Nejjednodušší způsob, jak zjistit, zda je použita zásada je tím, že vyžaduje, aby uživatel nastavit pin v zásadách.</span><span class="sxs-lookup"><span data-stu-id="b7d0c-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="b7d0c-113">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="b7d0c-113">For more information, see:</span></span>

[<span data-ttu-id="b7d0c-114">Nejčastější dotazy k řešení potíží s aplikací APP/MAM</span><span class="sxs-lookup"><span data-stu-id="b7d0c-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="b7d0c-115">Jak ověřit nastavení zásad ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="b7d0c-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="b7d0c-116">Principy časování doručování zásad ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="b7d0c-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="b7d0c-117">Jak sledovat zásady ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="b7d0c-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)