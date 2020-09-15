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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702896"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="2b0c4-102">Sledování podmíněného přístupu pro Exchange</span><span class="sxs-lookup"><span data-stu-id="2b0c4-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="2b0c4-103">Uživatelé s podmíněným přístupem budou dostávat e-mailové zprávy, pokud nesplňují požadavky na přístup vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2b0c4-104">Chcete-li vyřešit problém, doporučujeme jedno nebo více následujících řešení:</span><span class="sxs-lookup"><span data-stu-id="2b0c4-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="2b0c4-105">Pokud se předpokládá, že je zařízení zaregistrované, poraďte se s tím, že přejde do aplikace Portál společnosti a ověří, že se zobrazí na portálu společnosti.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2b0c4-106">Pokud to nepomůže, uživatel by měl zařízení zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="2b0c4-107">Na portálu Azure Portal přejděte na \*\* \> kompatibilitu zařízení\*\*.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2b0c4-108">V části **monitor** klikněte na položku **dodržování předpisů**.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="2b0c4-109">Zobrazte sestavu dodržování předpisů zařízení a ověřte, že zařízení uživatele je označené jako kompatibilní.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="2b0c4-110">Na portálu Azure Portal přejděte na \*\* \> kompatibilitu zařízení\*\*.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2b0c4-111">V části **Spravovat**klikněte na **zásady**.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="2b0c4-112">V seznamu zásad dodržování předpisů ověřte, zda je k zařízení uživatele přiřazen profil.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2b0c4-113">Pokud není přiřazen žádný profil, nebude moci Intune potvrdit jeho stav.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="2b0c4-114">Upravte přiřazení podmíněného přístupu uživatele.</span><span class="sxs-lookup"><span data-stu-id="2b0c4-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="2b0c4-115">V Azure Portalu přejděte na \*\* \> \> zásady podmíněného přístupu\*\* .</span><span class="sxs-lookup"><span data-stu-id="2b0c4-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="2b0c4-116">V seznamu vyberte zásadu</span><span class="sxs-lookup"><span data-stu-id="2b0c4-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="2b0c4-117">Klikněte na **Uživatelé a skupiny** .</span><span class="sxs-lookup"><span data-stu-id="2b0c4-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="2b0c4-118">Chcete-li určit určitou zásadu, přidejte ji do seznamu **zahrnutí** .</span><span class="sxs-lookup"><span data-stu-id="2b0c4-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="2b0c4-119">Chcete-li zajistit, aby některá osoba byla ze zásady vynechána, přidejte ji do seznamu **vyloučení** .</span><span class="sxs-lookup"><span data-stu-id="2b0c4-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="2b0c4-120">Další informace: [sledování zařízení podmíněného přístupu](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="2b0c4-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

