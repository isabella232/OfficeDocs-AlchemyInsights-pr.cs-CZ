---
title: Podmíněný přístup s Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931423"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="14461-102">Podmíněný přístup s Intune</span><span class="sxs-lookup"><span data-stu-id="14461-102">Conditional Access with Intune</span></span>

<span data-ttu-id="14461-103">Použití **podmíněného přístupu** s Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="14461-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="14461-104">Vytvořte **zásady dodržování předpisů** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a definujte nastavení, která musí být splněna, aby bylo zařízení považováno za vyhovující.</span><span class="sxs-lookup"><span data-stu-id="14461-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="14461-105">Zařízení musí mít například pin alespoň 6 číslic, aby bylo považováno za vyhovující.</span><span class="sxs-lookup"><span data-stu-id="14461-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="14461-106">Vytvořte **zásady podmíněného přístupu,** které definují, jaké prostředky jsou chráněny a jaké podmínky je třeba splnit pro přístup k těmto prostředkům.</span><span class="sxs-lookup"><span data-stu-id="14461-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="14461-107">Zařízení musí být [například](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) kompatibilní před přístupem k podnikovému e-mailu.</span><span class="sxs-lookup"><span data-stu-id="14461-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="14461-108">Ujistěte se, **že zásady dodržování předpisů** a **zásady podmíněného přístupu** jsou zaměřeny na požadované skupiny uživatelů.</span><span class="sxs-lookup"><span data-stu-id="14461-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="14461-109">To může vyžadovat vytvoření konkrétních skupin uživatelů ve službě Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14461-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="14461-110">**Užitečné odkazy:**</span><span class="sxs-lookup"><span data-stu-id="14461-110">**Helpful links:**</span></span>

[<span data-ttu-id="14461-111">Přehled dodržování předpisů pro zařízení</span><span class="sxs-lookup"><span data-stu-id="14461-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="14461-112">Poradce při potížích s certifikační autoritou</span><span class="sxs-lookup"><span data-stu-id="14461-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="14461-113">Zásady řešení potíží</span><span class="sxs-lookup"><span data-stu-id="14461-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="14461-114">Chcete-li chránit e-mail (Exchange online) před přístupem nekompatibilních zařízení, je třeba dodržovat oba dokumenty:</span><span class="sxs-lookup"><span data-stu-id="14461-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="14461-115">Ochrana přístupu k e-mailu ze zařízení pomocí služby EAS</span><span class="sxs-lookup"><span data-stu-id="14461-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="14461-116">Ochrana přístupu k e-mailu ze zařízení pomocí moderních klientů pro ověřování, jako je Outlook</span><span class="sxs-lookup"><span data-stu-id="14461-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)