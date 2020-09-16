---
title: Odstranění soukromého kanálu Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730908"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="1dfab-102">Odstranění soukromého kanálu Teams</span><span class="sxs-lookup"><span data-stu-id="1dfab-102">Delete a Teams private channel</span></span>

<span data-ttu-id="1dfab-103">Společnost Microsoft si uvědomila problém s odstraněním soukromého kanálu teams, pokud jsou u základního webu SharePointu povolené zásady uchovávání SharePointu.</span><span class="sxs-lookup"><span data-stu-id="1dfab-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="1dfab-104">Microsoft pracuje na opravě.</span><span class="sxs-lookup"><span data-stu-id="1dfab-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="1dfab-105">Do té doby můžete pomocí následujících zástupných řešení odstranit soukromý kanál.</span><span class="sxs-lookup"><span data-stu-id="1dfab-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="1dfab-106">**Vyloučení týmu/webu ze zásad uchovávání SharePointu**</span><span class="sxs-lookup"><span data-stu-id="1dfab-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="1dfab-107">Přejděte na portál pro správu Office 365 a v levém navigačním podokně vyberte **Zobrazit vše** .</span><span class="sxs-lookup"><span data-stu-id="1dfab-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="1dfab-108">V části **centra pro správu**přejděte na zásady ochrany před únikem dat **dodržování předpisů &**  >  **Data Loss Prevention**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="1dfab-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="1dfab-109">Identifikujte zásady, které platí pro sharepointové weby, a upravte zásadu tak, aby se sharepointový web obsahující privátní kanál nezahrnul do zásad uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="1dfab-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="1dfab-110">Uložte zásadu.</span><span class="sxs-lookup"><span data-stu-id="1dfab-110">Save the policy.</span></span>
    <span data-ttu-id="1dfab-111">Nastavení zásad může trvat až 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="1dfab-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="1dfab-112">Po vyloučení webu můžete soukromý kanál odstranit.</span><span class="sxs-lookup"><span data-stu-id="1dfab-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="1dfab-113">Na zařízení s Androidem  ***můžete soukromý*** kanál odstranit pomocí Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1dfab-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="1dfab-114">Informace o souvisejících SharePointu najdete [v článku nemůžete odstranit položky v SharePointu Online nebo OneDrivu pro firmy](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="1dfab-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>