---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685591"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="8cf0c-102">Blokování ověřování starší verze</span><span class="sxs-lookup"><span data-stu-id="8cf0c-102">Blocking legacy authentication</span></span>

<span data-ttu-id="8cf0c-103">Starší ověřování je termín, který odkazuje na žádost o ověření provedenou:</span><span class="sxs-lookup"><span data-stu-id="8cf0c-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="8cf0c-104">Starší klienti Office, kteří nepoužívají moderní ověřování (například klient Office 2010)</span><span class="sxs-lookup"><span data-stu-id="8cf0c-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="8cf0c-105">Všichni klienti používající starší poštovní protokoly, jako je IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="8cf0c-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="8cf0c-106">Další informace o blokování staršího ověřování a povolení moderního ověřování najdete v tématu [blokování ověřování starší verze](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="8cf0c-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="8cf0c-107">Výchozí nastavení zabezpečení v Azure Active Directory (Azure AD) usnadňuje bezpečnost a chrání vaši organizaci.</span><span class="sxs-lookup"><span data-stu-id="8cf0c-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="8cf0c-108">Výchozí nastavení zabezpečení obsahuje předem nakonfigurované nastavení zabezpečení pro běžné útoky.</span><span class="sxs-lookup"><span data-stu-id="8cf0c-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="8cf0c-109">Další informace o výchozích možnostech zabezpečení najdete v tématu [co jsou výchozí nastavení zabezpečení?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="8cf0c-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="8cf0c-110">**Poznámka**: Pokud se váš tenant vytvořil dne nebo po 22nd, 2019, je možné, že máte nové zabezpečené chování a že máte ve svém tenantovi povolené výchozí nastavení zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="8cf0c-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="8cf0c-111">V úsilí o ochranu všech našich uživatelů je pro všechny nově vytvořené klienty použito výchozí nastavení zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="8cf0c-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
