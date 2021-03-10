---
title: Použití podmíněného přístupu v Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692697"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="611f4-102">Použití podmíněného přístupu v Intune</span><span class="sxs-lookup"><span data-stu-id="611f4-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="611f4-103">Použití podmíněného přístupu v Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="611f4-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="611f4-104">Vytvořte zásady dodržování předpisů definující nastavení, která musí být splněná, aby bylo zařízení považované za zařízení dodržující předpisy. Aby bylo zařízení považované za zařízení dodržující předpisy, musí mít například kód PIN aspoň 6 číslic.</span><span class="sxs-lookup"><span data-stu-id="611f4-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="611f4-105">Vytvořte zásady podmíněného přístupu, které definují, které prostředky jsou chráněné a jaké podmínky musí být pro přístup k zdrojům splněné. Aby mělo například zařízení přístup k podnikovému e-mailu, musí být v souladu s předpisy.</span><span class="sxs-lookup"><span data-stu-id="611f4-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="611f4-106">Zajistěte, aby zásady dodržování předpisů a zásady podmíněného přístupu byly cílené na požadované skupiny uživatelů. To může vyžadovat vytvoření konkrétních skupin uživatelů v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="611f4-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="611f4-107">Další informace...</span><span class="sxs-lookup"><span data-stu-id="611f4-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
