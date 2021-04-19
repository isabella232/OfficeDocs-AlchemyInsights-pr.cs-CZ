---
title: Zásady podmíněného přístupu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817273"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="a3564-102">Zásady podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="a3564-102">Conditional Access policies</span></span>

<span data-ttu-id="a3564-103">Podmíněný přístup je funkce Azure AD, která vám umožní vynutit řízení přístupu k aplikacím ve vašem prostředí, a to na základě specifických podmínek a s možností správy z centrálního místa.</span><span class="sxs-lookup"><span data-stu-id="a3564-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="a3564-104">Přečtěte si další informace o [podmíněném přístupu Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="a3564-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="a3564-105">**Poznámka:** Pokud byl váš klient vytvořen po 21. říjnu 2019 a vám se neočekávaně zobrazuje vícefaktorové ověřování, pravděpodobně máte v klientovi povolená [výchozí nastavení zabezpečení](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="a3564-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="a3564-106">**Správa výchozích hodnot zabezpečení**</span><span class="sxs-lookup"><span data-stu-id="a3564-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="a3564-107">Přihlaste se do [Centra pro správu](https://go.microsoft.com/fwlink/p/?linkid=834822) pod uživatelským jménem a heslem globálního správce.</span><span class="sxs-lookup"><span data-stu-id="a3564-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="a3564-108">Přejděte na [Vlastnosti Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="a3564-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="a3564-109">V dolní části stránky klikněte na **Spravovat výchozí nastavení zabezpečení**.</span><span class="sxs-lookup"><span data-stu-id="a3564-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="a3564-110">Pokud chcete povolit výchozí nastavení zabezpečení, klikněte na **Ano**, pokud chcete zakázat výchozí zabezpečení, klikněte na **Ne**.</span><span class="sxs-lookup"><span data-stu-id="a3564-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
