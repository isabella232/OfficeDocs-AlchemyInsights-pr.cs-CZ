---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820171"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="fecd7-102">Blokování staršího ověřování</span><span class="sxs-lookup"><span data-stu-id="fecd7-102">Blocking legacy authentication</span></span>

<span data-ttu-id="fecd7-103">Starší ověřování je termín, který odkazuje na žádost o ověření ze strany:</span><span class="sxs-lookup"><span data-stu-id="fecd7-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="fecd7-104">Starší klienti Office, kteří používají moderní ověřování (například klient Office 2010).</span><span class="sxs-lookup"><span data-stu-id="fecd7-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="fecd7-105">Libovolný klient, který používá starší poštovní protokoly, například IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="fecd7-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="fecd7-106">Další informace o blokování staršího ověřování a povolení moderního ověřování najdete v tématu [Blokování staršího ověřování](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="fecd7-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="fecd7-107">Výchozí nastavení zabezpečení ve službě Azure Active Directory (Azure AD) usnadňují zabezpečení a pomáhají chránit vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="fecd7-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="fecd7-108">Výchozí nastavení zabezpečení obsahují předkonfigurované nastavení zabezpečení pro běžné útoky.</span><span class="sxs-lookup"><span data-stu-id="fecd7-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="fecd7-109">Další informace o výchozích nastaveních zabezpečení najdete v tématu [Co jsou výchozí nastavení zabezpečení?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="fecd7-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="fecd7-110">**Poznámka:** Pokud byl váš tenant vytvořen 22. října 2019 nebo po jeho uplynutí, je možné, že dochází k novému výchozímu chování zabezpečení a už máte ve svém tenantovi povolené výchozí nastavení zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="fecd7-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="fecd7-111">Ve snaze chránit všechny naše uživatele se pro všechny nové tenanty vytvářejí výchozí nastavení zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="fecd7-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
