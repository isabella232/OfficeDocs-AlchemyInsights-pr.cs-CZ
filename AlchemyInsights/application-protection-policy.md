---
title: Zásady ochrany aplikací
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716886"
---
# <a name="application-protection-policy"></a><span data-ttu-id="79d86-102">Zásady ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="79d86-102">Application protection policy</span></span>

<span data-ttu-id="79d86-103">Pokud se zásadou ochrany aplikací (aplikace) nepracujete, podívejte se na [Přehled zásad ochrany aplikací](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="79d86-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="79d86-104">Pokud chcete začít používat aplikaci, přečtěte si [článek Jak vytvořit a přiřadit zásady ochrany aplikací](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="79d86-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="79d86-105">Požadavky na zásady ochrany aplikací:</span><span class="sxs-lookup"><span data-stu-id="79d86-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="79d86-106">Uživatel má licenci Intune nebo EMS.</span><span class="sxs-lookup"><span data-stu-id="79d86-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="79d86-107">Uživatel patří do skupiny, která je cílová v zásadách ochrany aplikací.</span><span class="sxs-lookup"><span data-stu-id="79d86-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="79d86-108">Do chráněných aplikací na zařízení se přihlásí jenom jeden podnikový uživatel.</span><span class="sxs-lookup"><span data-stu-id="79d86-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="79d86-109">Aplikace implementovala [sadu Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="79d86-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="79d86-110">Seznam aplikací, které podporují sadu SDK, najdete v tématu [Microsoft Intune Protected Apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="79d86-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="79d86-111">Zásady platí, když uživatel, který splňuje výše uvedené požadavky, podepíše do aplikace Intune s podporou sady SDK.</span><span class="sxs-lookup"><span data-stu-id="79d86-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="79d86-112">Nejjednodušším způsobem, jak zjistit, jestli je zásada použitá, je to, když uživatel nastavil v zásadě PIN kód.</span><span class="sxs-lookup"><span data-stu-id="79d86-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="79d86-113">Další informace najdete tady:</span><span class="sxs-lookup"><span data-stu-id="79d86-113">For more information, see:</span></span>

[<span data-ttu-id="79d86-114">Časté otázky k aplikaci MAM a nejčastější dotazy</span><span class="sxs-lookup"><span data-stu-id="79d86-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="79d86-115">Jak ověřit nastavení zásad ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="79d86-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="79d86-116">Principy časování doručení zásad ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="79d86-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="79d86-117">Sledování zásad ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="79d86-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)