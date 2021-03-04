---
title: Sledování podmíněného přístupu Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427180"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="1bb6e-102">Sledování podmíněného přístupu Intune</span><span class="sxs-lookup"><span data-stu-id="1bb6e-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="1bb6e-103">Pokud uživatelé, na které podmíněný přístup zacílete, nesplňuje požadavky organizace na přístup, dostanou e-mail s oznámením.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="1bb6e-104">Jako řešení doporučujeme jedno nebo více z následujících řešení:</span><span class="sxs-lookup"><span data-stu-id="1bb6e-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="1bb6e-105">Pokud by už zařízení mělo být zaregistrované, poraďte uživateli, aby přecoval aplikaci Portál společnosti a ověřil, jestli se na portálu společnosti objeví.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="1bb6e-106">V tom případě musí uživatel zařízení zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="1bb6e-107">Na portálu Azure Portal přejděte na Dodržování **předpisů**  >  **zařízením** Intune.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="1bb6e-108">Pokud chcete zobrazit sestavu o dodržování předpisů zařízením a ověřit, jestli je zařízení uživatele označené jako zařízení dodržující předpisy, klikněte v části **Monitor** na **Dodržování předpisů zařízením.**</span><span class="sxs-lookup"><span data-stu-id="1bb6e-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="1bb6e-109">Na portálu Azure Portal přejděte na Dodržování **předpisů**  >  **zařízením** Intune.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="1bb6e-110">V **části Spravovat klikněte** na **Zásady.**</span><span class="sxs-lookup"><span data-stu-id="1bb6e-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="1bb6e-111">V seznamu zásad dodržování předpisů ověřte, jestli má zařízení uživatele přiřazený profil.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="1bb6e-112">Pokud není žádný profil přiřazený, nebude moct Intune ověřit stav dodržování předpisů zařízení.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="1bb6e-113">Upravte přiřazení podmíněného přístupu uživatele.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="1bb6e-114">Na portálu Azure Portal přejděte na Zásady podmíněného přístupu **Intune,** vyberte zásadu ze seznamu a klikněte na  >    >  Uživatelé a **skupiny.**</span><span class="sxs-lookup"><span data-stu-id="1bb6e-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="1bb6e-115">Pokud chcete určité zásady na někoho zacílit, přidejte ho do **seznamu Zahrnout.**</span><span class="sxs-lookup"><span data-stu-id="1bb6e-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="1bb6e-116">Pokud chcete zajistit, aby byla osoba ze zásad vynechána, přidejte ji do **seznamu Vyloučit.**</span><span class="sxs-lookup"><span data-stu-id="1bb6e-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="1bb6e-117">**Užitečné odkazy:**</span><span class="sxs-lookup"><span data-stu-id="1bb6e-117">**Helpful links:**</span></span>

- [<span data-ttu-id="1bb6e-118">Přehled dodržování předpisů zařízením</span><span class="sxs-lookup"><span data-stu-id="1bb6e-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="1bb6e-119">Řešení potíží s CA</span><span class="sxs-lookup"><span data-stu-id="1bb6e-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="1bb6e-120">Zásady pro řešení potíží</span><span class="sxs-lookup"><span data-stu-id="1bb6e-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="1bb6e-121">Monitorování dodržování předpisů zařízením Intune</span><span class="sxs-lookup"><span data-stu-id="1bb6e-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="1bb6e-122">Tyto kroky jsou užitečné jenom při řešení potíží s podmíněným přístupem funkce Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="1bb6e-123">Taky je možné umístit zařízení do karantény, které zablokuje přístup k e-mailu pomocí zásad Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bb6e-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="1bb6e-124">Další informace o správě zařízení Exchange najdete [**tady.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="1bb6e-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
