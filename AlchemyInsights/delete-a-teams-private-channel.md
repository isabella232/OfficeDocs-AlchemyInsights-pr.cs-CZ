---
title: Odstranění soukromého kanálu Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438836"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="3392e-102">Odstranění soukromého kanálu Teams</span><span class="sxs-lookup"><span data-stu-id="3392e-102">Delete a Teams private channel</span></span>

<span data-ttu-id="3392e-103">Společnost Microsoft si je vědoma problému s odstraněním soukromého kanálu Teams, pokud máte pro základní web služby SharePoint povolené zásady uchovávání informací sharepointu.</span><span class="sxs-lookup"><span data-stu-id="3392e-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="3392e-104">Společnost Microsoft pracuje na opravě.</span><span class="sxs-lookup"><span data-stu-id="3392e-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="3392e-105">Do té doby můžete použít následující zástupná řešení k odstranění soukromého kanálu.</span><span class="sxs-lookup"><span data-stu-id="3392e-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="3392e-106">**Vylučte kolekci týmu nebo webu ze zásad uchovávání informací sharepointu.**</span><span class="sxs-lookup"><span data-stu-id="3392e-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="3392e-107">Přejděte na portál pro správu Office 365 a v levém navigačním podokně vyberte **Zobrazit vše.**</span><span class="sxs-lookup"><span data-stu-id="3392e-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="3392e-108">V části **Centra pro správu**přejděte na **Bezpečnostní &**  >  **zásady prevence ztrát na datech**dodržování  >  **předpisů**.</span><span class="sxs-lookup"><span data-stu-id="3392e-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="3392e-109">Identifikujte všechny zásady, které se vztahují k webům Služby SharePoint, a upravte zásady tak, aby web Služby SharePoint pro tým obsahující soukromý kanál nebyl zahrnut do zásad uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="3392e-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="3392e-110">Uložte zásady.</span><span class="sxs-lookup"><span data-stu-id="3392e-110">Save the policy.</span></span>
    <span data-ttu-id="3392e-111">Nastavení zásad může trvat až 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="3392e-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="3392e-112">Po vyloučení webu můžete soukromý kanál odstranit.</span><span class="sxs-lookup"><span data-stu-id="3392e-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="3392e-113">Soukromý kanál ***můžete*** odstranit pomocí Microsoft Teams na zařízení s Androidem.</span><span class="sxs-lookup"><span data-stu-id="3392e-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="3392e-114">Související sharepointové informace najdete [v tématu Nelze odstranit položky v SharePointu Online nebo OneDrivu pro firmy](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="3392e-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>