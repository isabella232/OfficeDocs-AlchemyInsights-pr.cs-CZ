---
title: O Yammer správců
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/22/2021
ms.locfileid: "51035732"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="11e12-102">O Yammer správců</span><span class="sxs-lookup"><span data-stu-id="11e12-102">About Yammer admins</span></span>

<span data-ttu-id="11e12-103">**Správci sítě**</span><span class="sxs-lookup"><span data-stu-id="11e12-103">**Network admins**</span></span>

<span data-ttu-id="11e12-104">Globální správci se automaticky propagují na roli ověřeného správce v Yammer síti.</span><span class="sxs-lookup"><span data-stu-id="11e12-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="11e12-105">V následujících případech se tato propagační akce nemusí vyskytnout správně:</span><span class="sxs-lookup"><span data-stu-id="11e12-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="11e12-106">Existuje Yammer sítí a správce je přihlášený k nesprávnému.</span><span class="sxs-lookup"><span data-stu-id="11e12-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="11e12-107">[Sloučení sítě](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) je nutné, abyste se do jedné Yammer sítě.</span><span class="sxs-lookup"><span data-stu-id="11e12-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="11e12-108">Používá se Azure PIM.</span><span class="sxs-lookup"><span data-stu-id="11e12-108">Azure PIM is being used.</span></span> <span data-ttu-id="11e12-109">Uživatel nemusí být povýšen na globálního správce dost dlouho, aby k propagační akci došlo.</span><span class="sxs-lookup"><span data-stu-id="11e12-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="11e12-110">Budoucí aktualizace systému Yammer tento problém vyřešit, ale nejlepší je, když uživatele zvýšíte na globálního správce ručně.</span><span class="sxs-lookup"><span data-stu-id="11e12-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="11e12-111">Se sítí Yammer existuje problém se synchronizací.</span><span class="sxs-lookup"><span data-stu-id="11e12-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="11e12-112">V takovém případě bude vyžadována žádost o podporu pro další vyšetřování.</span><span class="sxs-lookup"><span data-stu-id="11e12-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="11e12-113">Další informace o rolích Yammer najdete v tématu [Správa Yammer správců](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="11e12-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="11e12-114">**Správci skupin**</span><span class="sxs-lookup"><span data-stu-id="11e12-114">**Group admins**</span></span>

<span data-ttu-id="11e12-115">Správci skupin pro skupiny připojené k Microsoftu 365 se synchronizují s členstvím ve skupině z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="11e12-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="11e12-116">U velkých skupin může tato synchronizace trvat delší dobu.</span><span class="sxs-lookup"><span data-stu-id="11e12-116">For large groups, this sync can take an extended period.</span></span>
