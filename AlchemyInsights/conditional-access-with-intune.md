---
title: Podmíněný přístup s Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807652"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="1c71c-102">Podmíněný přístup s Intune</span><span class="sxs-lookup"><span data-stu-id="1c71c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="1c71c-103">Použití  **podmíněného přístupu**  s Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="1c71c-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="1c71c-104">Vytvořením  **zásad dodržování předpisů**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) definujte nastavení, která musí být splněná, než se zařízení považuje za kompatibilní.</span><span class="sxs-lookup"><span data-stu-id="1c71c-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="1c71c-105">Například zařízení musí mít PIN kód alespoň 6 číslic, než se považuje za vyhovující.</span><span class="sxs-lookup"><span data-stu-id="1c71c-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="1c71c-106">Vytvořte **zásadu podmíněného přístupu**  definující prostředky, které se chrání, a jaké podmínky je třeba pro přístup k těmto prostředkům splnit.</span><span class="sxs-lookup"><span data-stu-id="1c71c-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="1c71c-107">Před [přístupem do](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) firemních e-mailů musí být zařízení kompatibilní.</span><span class="sxs-lookup"><span data-stu-id="1c71c-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="1c71c-108">Zajistěte, aby **zásady dodržování předpisů**  a  **zásady podmíněného přístupu**  byly cílené na požadované skupiny uživatelů.</span><span class="sxs-lookup"><span data-stu-id="1c71c-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="1c71c-109">To by mohlo vyžadovat vytvoření určitých skupin uživatelů v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1c71c-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="1c71c-110">**Užitečné odkazy:**</span><span class="sxs-lookup"><span data-stu-id="1c71c-110">**Helpful links:**</span></span>

[<span data-ttu-id="1c71c-111">Přehled dodržování předpisů zařízení</span><span class="sxs-lookup"><span data-stu-id="1c71c-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="1c71c-112">Poradce při potížích</span><span class="sxs-lookup"><span data-stu-id="1c71c-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="1c71c-113">Zásady řešení potíží</span><span class="sxs-lookup"><span data-stu-id="1c71c-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="1c71c-114">Chcete-li chránit E-mail (Exchange Online) z Accessu neodpovídajícími zařízeními, musí být dodržovány oba dokumenty:</span><span class="sxs-lookup"><span data-stu-id="1c71c-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="1c71c-115">Ochrana přístupu k e-mailu ze zařízení pomocí EAS</span><span class="sxs-lookup"><span data-stu-id="1c71c-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="1c71c-116">Ochrana e-mailových zpráv ze zařízení pomocí moderních klientů ověřování, jako je Outlook</span><span class="sxs-lookup"><span data-stu-id="1c71c-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)