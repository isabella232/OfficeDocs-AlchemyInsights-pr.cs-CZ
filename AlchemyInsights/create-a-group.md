---
title: Vytvoření skupiny
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088575"
---
# <a name="create-a-group"></a><span data-ttu-id="33357-102">Vytvoření skupiny</span><span class="sxs-lookup"><span data-stu-id="33357-102">Create a group</span></span>

<span data-ttu-id="33357-103">Toto téma popisuje vytvoření skupiny.</span><span class="sxs-lookup"><span data-stu-id="33357-103">This topic describes group creation.</span></span>

<span data-ttu-id="33357-104">**Oprávnění k vytvoření skupiny**</span><span class="sxs-lookup"><span data-stu-id="33357-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="33357-105">Zkontrolujte, jestli máte oprávnění vytvořit novou skupinu.</span><span class="sxs-lookup"><span data-stu-id="33357-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="33357-106">Globální správci můžou zakázat vytváření skupin na portálu Azure nebo v panelu přístup.</span><span class="sxs-lookup"><span data-stu-id="33357-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="33357-107">Abyste mohli vytvořit novou skupinu nebo vám udělit odpovídající oprávnění, budete možná potřebovat správce.</span><span class="sxs-lookup"><span data-stu-id="33357-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="33357-108">**Správa oprávnění pro vytváření skupin**</span><span class="sxs-lookup"><span data-stu-id="33357-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="33357-109">Globální Správci mohou spravovat oprávnění k vytváření skupin (z bezpečnostních důvodů) nebo skupiny Office 365 vytvořené na portálu Azure Portal nebo v panelu přístup tak, že výběrem možnosti "uživatelé můžou vytvářet skupiny zabezpečení v portálech Azure" nebo "uživatelé můžou vytvářet skupiny Office **365 v Azure** portáls"  >  **(nastavení)**.</span><span class="sxs-lookup"><span data-stu-id="33357-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="33357-110">Pokud máte licenci Azure Active Directory P1 Premium, můžete vytvářet skupiny také pro výběr skupiny uživatelů.</span><span class="sxs-lookup"><span data-stu-id="33357-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="33357-111">**Zakázání uvítacího oznámení pro nové členy skupiny Office 365**</span><span class="sxs-lookup"><span data-stu-id="33357-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="33357-112">Uvítací oznámení, které se uživatelům přidají do skupin Office 365, můžete zakázat nastavením **UnifiedGroupWelcomeMessageEnabled** na false v PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="33357-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="33357-113">Přečtěte [si toto nastavení.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="33357-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

