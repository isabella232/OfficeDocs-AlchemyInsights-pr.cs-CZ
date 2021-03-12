---
title: Podmíněný přístup pomocí Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704779"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="aa950-102">Podmíněný přístup pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="aa950-102">Conditional Access with Intune</span></span>

<span data-ttu-id="aa950-103">Použití  **podmíněného přístupu**  v Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="aa950-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="aa950-104">Vytvořte zásady  **dodržování předpisů** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)definující nastavení, která musí být splněná, aby bylo zařízení považované za zařízení dodržující předpisy.</span><span class="sxs-lookup"><span data-stu-id="aa950-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="aa950-105">Aby bylo zařízení považované za zařízení dodržující předpisy, musí mít například kód PIN aspoň 6 číslic.</span><span class="sxs-lookup"><span data-stu-id="aa950-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="aa950-106">Vytvořte zásady **podmíněného přístupu,**  které definují, které prostředky jsou chráněné a jaké podmínky musí být pro přístup k zdrojům splněné.</span><span class="sxs-lookup"><span data-stu-id="aa950-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="aa950-107">[Aby mělo například zařízení](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  přístup k podnikovému e-mailu, musí být v souladu s předpisy.</span><span class="sxs-lookup"><span data-stu-id="aa950-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="aa950-108">**Zajistěte, aby zásady dodržování** předpisů a zásady **podmíněného** přístupu byly cílené na požadované skupiny uživatelů.</span><span class="sxs-lookup"><span data-stu-id="aa950-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="aa950-109">To může vyžadovat vytvoření konkrétních skupin uživatelů v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aa950-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="aa950-110">**Užitečné odkazy:**</span><span class="sxs-lookup"><span data-stu-id="aa950-110">**Helpful links:**</span></span>

[<span data-ttu-id="aa950-111">Přehled dodržování předpisů zařízením</span><span class="sxs-lookup"><span data-stu-id="aa950-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="aa950-112">Řešení potíží s CA</span><span class="sxs-lookup"><span data-stu-id="aa950-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="aa950-113">Zásady pro řešení potíží</span><span class="sxs-lookup"><span data-stu-id="aa950-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="aa950-114">Pokud chcete e-mail (Exchange Online) chránit před přístupem zařízení, která nejsou s tím, jak mají být, musí následovat oba dokumenty:</span><span class="sxs-lookup"><span data-stu-id="aa950-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="aa950-115">Ochrana přístupu k e-mailu ze zařízení pomocí EAS</span><span class="sxs-lookup"><span data-stu-id="aa950-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="aa950-116">Ochrana přístupu k e-mailu ze zařízení pomocí moderních ověřovacích klientů, jako je outlook</span><span class="sxs-lookup"><span data-stu-id="aa950-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)