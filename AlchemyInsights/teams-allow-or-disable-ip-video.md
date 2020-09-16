---
title: Týmy povolují nebo zakazují video IP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670177"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="51b75-102">Týmy povolují nebo zakazují video IP</span><span class="sxs-lookup"><span data-stu-id="51b75-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="51b75-103">**Změna nebo vytvoření zásady schůzky**</span><span class="sxs-lookup"><span data-stu-id="51b75-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="51b75-104">Pokud chcete změnit nebo vytvořit zásadu schůzky, přejděte do **centra pro správu Microsoft teams > schůzky > zásady schůzky**.</span><span class="sxs-lookup"><span data-stu-id="51b75-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="51b75-105">Ze seznamu vyberte zásady nebo klikněte na **Přidat**.</span><span class="sxs-lookup"><span data-stu-id="51b75-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="51b75-106">Jestliže vytváříte nové zásady, pojmenujte je a přidejte popis.</span><span class="sxs-lookup"><span data-stu-id="51b75-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="51b75-107">Název nesmí obsahovat speciální znaky ani mít víc než 64 znaků.</span><span class="sxs-lookup"><span data-stu-id="51b75-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="51b75-108">Zvolte požadovaná nastavení a potom klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="51b75-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="51b75-109">Řekněme třeba, že máte hodně uživatelů a chcete omezit šířku pásma, která by měla schůzka vyžadovat.</span><span class="sxs-lookup"><span data-stu-id="51b75-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="51b75-110">Vytvoříte nové vlastní zásady nazvané Omezená šířka pásma a zakážete následující nastavení:</span><span class="sxs-lookup"><span data-stu-id="51b75-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="51b75-111">V části **Zvuk a video**:</span><span class="sxs-lookup"><span data-stu-id="51b75-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="51b75-112">Vypnete možnost Povolit nahrávání do cloudu.</span><span class="sxs-lookup"><span data-stu-id="51b75-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="51b75-113">Vypnete možnost Povolit IP video.</span><span class="sxs-lookup"><span data-stu-id="51b75-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="51b75-114">Pak zásadu přiřadíte uživatelům.</span><span class="sxs-lookup"><span data-stu-id="51b75-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="51b75-115">**Přiřazení zásady schůzky uživatelům**</span><span class="sxs-lookup"><span data-stu-id="51b75-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="51b75-116">V levém navigačním panelu centra pro správu Microsoft Teams přejděte na **Uživatele** a potom klikněte na uživatele.</span><span class="sxs-lookup"><span data-stu-id="51b75-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="51b75-117">Kliknutím vlevo od uživatelského jména vyberte uživatele a pak klikněte na **Upravit nastavení**.</span><span class="sxs-lookup"><span data-stu-id="51b75-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="51b75-118">V části **zásady schůzky**vyberte zásadu, kterou chcete přiřadit, a pak klikněte na **použít**.</span><span class="sxs-lookup"><span data-stu-id="51b75-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="51b75-119">Další informace najdete v tématu [Správa zásad schůzky v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="51b75-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
