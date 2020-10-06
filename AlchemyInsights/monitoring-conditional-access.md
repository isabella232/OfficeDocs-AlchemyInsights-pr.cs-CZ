---
title: Sledování podmíněného přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366421"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="b980e-102">Sledování podmíněného přístupu pro Exchange</span><span class="sxs-lookup"><span data-stu-id="b980e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="b980e-103">Uživatelé s podmíněným přístupem budou dostávat e-mailové zprávy, pokud nesplňují požadavky na přístup vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="b980e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b980e-104">Chcete-li vyřešit problém, doporučujeme jedno nebo více následujících řešení:</span><span class="sxs-lookup"><span data-stu-id="b980e-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="b980e-105">Pokud se předpokládá, že je zařízení zaregistrované, poraďte se s tím, že přejde do aplikace Portál společnosti a ověří, že se zobrazí na portálu společnosti.</span><span class="sxs-lookup"><span data-stu-id="b980e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b980e-106">Pokud to nepomůže, uživatel by měl zařízení zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="b980e-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="b980e-107">Na Azure Portal přejděte na Intune > dodržování předpisů zařízení.</span><span class="sxs-lookup"><span data-stu-id="b980e-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="b980e-108">V části Monitor klikněte na položku dodržování předpisů.</span><span class="sxs-lookup"><span data-stu-id="b980e-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="b980e-109">Zobrazte sestavu dodržování předpisů zařízení a ověřte, že zařízení uživatele je označené jako kompatibilní.</span><span class="sxs-lookup"><span data-stu-id="b980e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="b980e-110">Na Azure Portal přejděte na Intune > dodržování předpisů zařízení.</span><span class="sxs-lookup"><span data-stu-id="b980e-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="b980e-111">V části Spravovat klikněte na zásady.</span><span class="sxs-lookup"><span data-stu-id="b980e-111">Under Manage, click Policies.</span></span> <span data-ttu-id="b980e-112">V seznamu zásad dodržování předpisů ověřte, zda je k zařízení uživatele přiřazen profil.</span><span class="sxs-lookup"><span data-stu-id="b980e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b980e-113">Pokud není přiřazen žádný profil, nebude moci Intune potvrdit jeho stav.</span><span class="sxs-lookup"><span data-stu-id="b980e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="b980e-114">Upravte přiřazení podmíněného přístupu uživatele.</span><span class="sxs-lookup"><span data-stu-id="b980e-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="b980e-115">V Azure Portal **přejděte na**  >  **zásady podmíněného přístupu**  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="b980e-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="b980e-116">V seznamu vyberte zásadu.</span><span class="sxs-lookup"><span data-stu-id="b980e-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="b980e-117">Klikněte na uživatelé a skupiny.</span><span class="sxs-lookup"><span data-stu-id="b980e-117">Click Users and groups.</span></span>
4. <span data-ttu-id="b980e-118">Chcete-li určit určitou zásadu, přidejte ji do seznamu zahrnutí.</span><span class="sxs-lookup"><span data-stu-id="b980e-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="b980e-119">Chcete-li zajistit, aby některá osoba byla ze zásady vynechána, přidejte ji do seznamu vyloučení.</span><span class="sxs-lookup"><span data-stu-id="b980e-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="b980e-120">Užitečné odkazy:</span><span class="sxs-lookup"><span data-stu-id="b980e-120">Helpful links:</span></span>

[<span data-ttu-id="b980e-121">Přehled dodržování předpisů zařízení</span><span class="sxs-lookup"><span data-stu-id="b980e-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="b980e-122">Poradce při potížích</span><span class="sxs-lookup"><span data-stu-id="b980e-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b980e-123">Zásady řešení potíží</span><span class="sxs-lookup"><span data-stu-id="b980e-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="b980e-124">Monitorování dodržování předpisů zařízení</span><span class="sxs-lookup"><span data-stu-id="b980e-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="b980e-125">Poznámka: Tento postup je užitečný jenom při odstraňování potíží s podmíněným přístupem Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b980e-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="b980e-126">Je taky možné zablokovat zařízení blokující přístup k e-mailu pomocí zásad Exchange.</span><span class="sxs-lookup"><span data-stu-id="b980e-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="b980e-127">Další informace o správě zařízení Exchange najdete [tady](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="b980e-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
