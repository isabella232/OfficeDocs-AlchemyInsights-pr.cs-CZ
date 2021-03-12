---
title: Monitorování podmíněného přístupu
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708667"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="9fd89-102">Monitorování podmíněného přístupu pro Exchange</span><span class="sxs-lookup"><span data-stu-id="9fd89-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="9fd89-103">Pokud uživatelé, na které podmíněný přístup zacílete, nesplňuje požadavky organizace na přístup, dostanou e-mail s oznámením.</span><span class="sxs-lookup"><span data-stu-id="9fd89-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9fd89-104">Jako řešení doporučujeme jedno nebo více z následujících řešení:</span><span class="sxs-lookup"><span data-stu-id="9fd89-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="9fd89-105">Pokud by už zařízení mělo být zaregistrované, poraďte uživateli, aby přecoval aplikaci Portál společnosti a ověřil, jestli se na portálu společnosti objeví.</span><span class="sxs-lookup"><span data-stu-id="9fd89-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9fd89-106">Pokud ne, měl by uživatel zařízení zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="9fd89-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="9fd89-107">Na portálu Azure Portal přejděte na Intune > dodržování předpisů zařízením.</span><span class="sxs-lookup"><span data-stu-id="9fd89-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="9fd89-108">V části Monitorovat klikněte na Dodržování předpisů zařízením.</span><span class="sxs-lookup"><span data-stu-id="9fd89-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="9fd89-109">Prohlédněte si sestavu o dodržování předpisů zařízením a ověřte, jestli je zařízení uživatele označené jako zařízení dodržující předpisy.</span><span class="sxs-lookup"><span data-stu-id="9fd89-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="9fd89-110">Na portálu Azure Portal přejděte na Intune > dodržování předpisů zařízením.</span><span class="sxs-lookup"><span data-stu-id="9fd89-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="9fd89-111">V části Spravovat klikněte na Zásady.</span><span class="sxs-lookup"><span data-stu-id="9fd89-111">Under Manage, click Policies.</span></span> <span data-ttu-id="9fd89-112">V seznamu zásad dodržování předpisů ověřte, jestli má zařízení uživatele přiřazený profil.</span><span class="sxs-lookup"><span data-stu-id="9fd89-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9fd89-113">Pokud není žádný profil přiřazený, nebude moct Intune ověřit stav dodržování předpisů zařízení.</span><span class="sxs-lookup"><span data-stu-id="9fd89-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="9fd89-114">Upravte přiřazení podmíněného přístupu uživatele.</span><span class="sxs-lookup"><span data-stu-id="9fd89-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="9fd89-115">Na portálu Azure Portal přejděte na Zásady  >  **podmíněného přístupu**  >  Intune.</span><span class="sxs-lookup"><span data-stu-id="9fd89-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="9fd89-116">V seznamu vyberte zásadu.</span><span class="sxs-lookup"><span data-stu-id="9fd89-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="9fd89-117">Klikněte na Uživatelé a skupiny.</span><span class="sxs-lookup"><span data-stu-id="9fd89-117">Click Users and groups.</span></span>
4. <span data-ttu-id="9fd89-118">Pokud chcete určité zásady na někoho zacílit, přidejte ho do seznamu Zahrnout.</span><span class="sxs-lookup"><span data-stu-id="9fd89-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="9fd89-119">Pokud chcete zajistit, aby byla osoba ze zásad vynechána, přidejte ji do seznamu Vyloučit.</span><span class="sxs-lookup"><span data-stu-id="9fd89-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="9fd89-120">Užitečné odkazy:</span><span class="sxs-lookup"><span data-stu-id="9fd89-120">Helpful links:</span></span>

[<span data-ttu-id="9fd89-121">Přehled dodržování předpisů zařízením</span><span class="sxs-lookup"><span data-stu-id="9fd89-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9fd89-122">Řešení potíží s CA</span><span class="sxs-lookup"><span data-stu-id="9fd89-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9fd89-123">Zásady pro řešení potíží</span><span class="sxs-lookup"><span data-stu-id="9fd89-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="9fd89-124">Monitorování dodržování předpisů zařízením Intune</span><span class="sxs-lookup"><span data-stu-id="9fd89-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="9fd89-125">Poznámka: Tento postup je užitečný jenom při řešení potíží s podmíněným přístupem funkce Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9fd89-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="9fd89-126">Taky je možné umístit zařízení do karantény, které zablokuje přístup k e-mailu pomocí zásad Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fd89-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="9fd89-127">Další informace o správě zařízení exchange najdete [tady]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)</span><span class="sxs-lookup"><span data-stu-id="9fd89-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
