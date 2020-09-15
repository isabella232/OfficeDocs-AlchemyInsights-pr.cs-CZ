---
title: Dynamics 365 – chybný řídicí panel v rozhraní Dynamics 365 Unified
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711268"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="ff97f-102">Chybný řídicí panel zobrazený v aplikaci Dynamics 365 Unified Interface</span><span class="sxs-lookup"><span data-stu-id="ff97f-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="ff97f-103">Existuje několik důvodů, proč se může zobrazit jiný řídicí panel, než očekáváte:</span><span class="sxs-lookup"><span data-stu-id="ff97f-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="ff97f-104">Uživatel nastavil výchozí uživatelský řídicí panel</span><span class="sxs-lookup"><span data-stu-id="ff97f-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="ff97f-105">Výchozí uživatelský řídicí panel se obvykle dá nastavit, pokud se na panelu příkazů řídicí panel nezobrazí tlačítko **nastavit jako výchozí** .</span><span class="sxs-lookup"><span data-stu-id="ff97f-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="ff97f-106">Výchozí řídicí panel uživatele přepíše všechny ostatní výchozí řídicí panely, a to i v případě, že výchozí řídicí panel uživatele není aktuální aplikací.</span><span class="sxs-lookup"><span data-stu-id="ff97f-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="ff97f-107">Pomocí následujícího zástupného řešení zrušte výchozí řídicí panel.</span><span class="sxs-lookup"><span data-stu-id="ff97f-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="ff97f-108">Vytvořte nový osobní řídicí panel.</span><span class="sxs-lookup"><span data-stu-id="ff97f-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="ff97f-109">Nastavte si nový řídicí panel jako výchozí.</span><span class="sxs-lookup"><span data-stu-id="ff97f-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="ff97f-110">Odstraňte tento řídicí panel.</span><span class="sxs-lookup"><span data-stu-id="ff97f-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="ff97f-111">V prvku Sitemap je nastaven řídicí panel</span><span class="sxs-lookup"><span data-stu-id="ff97f-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="ff97f-112">Možná jste nastavili výchozí řídicí panel organizace výběrem řídicího panelu a zvolením možnosti nastavit jako výchozí v části přizpůsobit systém.</span><span class="sxs-lookup"><span data-stu-id="ff97f-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="ff97f-113">Ale řídicí panel definovaný v Návrháři mapy webu bude mít při přístupu k tomuto řídicímu panelu přednost.</span><span class="sxs-lookup"><span data-stu-id="ff97f-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="ff97f-114">Pokud chcete, aby uživatelé viděli řídicí panel, který jste nastavili jako výchozí, můžete:</span><span class="sxs-lookup"><span data-stu-id="ff97f-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="ff97f-115">Nastavení tohoto řídicího panelu v článku Mapa stránek</span><span class="sxs-lookup"><span data-stu-id="ff97f-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="ff97f-116">Odebrání přístupu k řídicímu panelu mapy webu pro tyto uživatele</span><span class="sxs-lookup"><span data-stu-id="ff97f-116">Remove access to the sitemap defined dashboard for those users</span></span>
