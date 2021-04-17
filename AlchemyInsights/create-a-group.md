---
title: Vytvoření skupiny
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816341"
---
# <a name="create-a-group"></a><span data-ttu-id="afbc9-102">Vytvoření skupiny</span><span class="sxs-lookup"><span data-stu-id="afbc9-102">Create a group</span></span>

<span data-ttu-id="afbc9-103">Toto téma popisuje vytváření skupin.</span><span class="sxs-lookup"><span data-stu-id="afbc9-103">This topic describes group creation.</span></span>

<span data-ttu-id="afbc9-104">**Oprávnění k vytvoření skupiny**</span><span class="sxs-lookup"><span data-stu-id="afbc9-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="afbc9-105">Ujistěte se, že máte oprávnění k vytvoření nové skupiny.</span><span class="sxs-lookup"><span data-stu-id="afbc9-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="afbc9-106">Globální správci můžou vytváření skupin zakázat na portálu Azure portal nebo na přístupových panelech.</span><span class="sxs-lookup"><span data-stu-id="afbc9-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="afbc9-107">Možná budete potřebovat správce, který za vás vytvoří novou skupinu nebo vám dá příslušná oprávnění.</span><span class="sxs-lookup"><span data-stu-id="afbc9-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="afbc9-108">**Správa oprávnění pro vytváření skupin**</span><span class="sxs-lookup"><span data-stu-id="afbc9-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="afbc9-109">Globální správci můžou spravovat oprávnění k vytváření skupin (z důvodů souvisejících se zabezpečením) nebo skupiny Office 365 vytvořené na portálu Azure portal nebo na accessových panelech tak, že zvolí "Uživatelé můžou vytvářet skupiny zabezpečení na portálech Azure" nebo "Uživatelé můžou vytvářet skupiny Office 365 na portálech Azure" v části Všechny skupiny – obecné  >  **(Nastavení)**.</span><span class="sxs-lookup"><span data-stu-id="afbc9-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="afbc9-110">Pokud máte licenci Azure Active Directory P1 Premium, můžete omezit vytváření skupin na výběr skupiny uživatelů.</span><span class="sxs-lookup"><span data-stu-id="afbc9-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="afbc9-111">**Zakázání uvítacího oznámení pro nové členy skupiny Office 365**</span><span class="sxs-lookup"><span data-stu-id="afbc9-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="afbc9-112">Uvítací oznámení odeslané uživatelům, kteří jsou přidáni do skupin Office 365, můžete zakázat nastavením **funkce UnifiedGroupWelcomeMessageEnabled** na False v PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="afbc9-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="afbc9-113">Další informace o tomto nastavení [najdete tady.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="afbc9-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

