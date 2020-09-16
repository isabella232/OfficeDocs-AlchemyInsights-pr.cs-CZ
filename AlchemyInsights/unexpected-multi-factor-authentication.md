---
title: Neočekávané vícefaktorové ověřování
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 48303d5b408cbdb243ec45dc4c80ac9a83f273a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689515"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="a341d-102">Neočekávané vícefaktorové ověřování</span><span class="sxs-lookup"><span data-stu-id="a341d-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="a341d-103">Pokud byl váš klient vytvořen po 21. říjnu 2019 a vám se neočekávaně zobrazuje vícefaktorové ověřování, pravděpodobně máte v klientovi povolená [výchozí nastavení zabezpečení](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="a341d-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="a341d-104">Správa výchozích hodnot zabezpečení:</span><span class="sxs-lookup"><span data-stu-id="a341d-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="a341d-105">Přihlaste se do [Centra pro správu](https://go.microsoft.com/fwlink/p/?linkid=834822) pod uživatelským jménem a heslem globálního správce.</span><span class="sxs-lookup"><span data-stu-id="a341d-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="a341d-106">Přejděte na [Vlastnosti Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="a341d-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="a341d-107">V dolní části stránky klikněte na **Spravovat výchozí nastavení zabezpečení**.</span><span class="sxs-lookup"><span data-stu-id="a341d-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="a341d-108">Pokud chcete povolit výchozí nastavení zabezpečení, klikněte na **Ano**, pokud chcete zakázat výchozí zabezpečení, klikněte na **Ne**.</span><span class="sxs-lookup"><span data-stu-id="a341d-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
