---
title: 618 zásady sdílení kalendáře
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684223"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="78979-102">Chyba zásad při sdílení kalendáře</span><span class="sxs-lookup"><span data-stu-id="78979-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="78979-103">Podle situace proveďte jednu z následujících akcí:</span><span class="sxs-lookup"><span data-stu-id="78979-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="78979-104">Připojení k Exchangi Online pomocí vzdáleného PowerShellu</span><span class="sxs-lookup"><span data-stu-id="78979-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="78979-105">Další informace najdete v článku [připojení k Exchangi Online pomocí vzdáleného PowerShellu](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="78979-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="78979-106">Na místním serveru otevřete prostředí Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="78979-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="78979-107">Určete zásady sdílení přiřazené uživateli.</span><span class="sxs-lookup"><span data-stu-id="78979-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="78979-108">To provedete tak, že spustíte následující příkaz a navrátili jste vrácenou zásadu:</span><span class="sxs-lookup"><span data-stu-id="78979-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="78979-109">Aktualizace zásad sdílení pro uživatele</span><span class="sxs-lookup"><span data-stu-id="78979-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="78979-110">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="78979-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="78979-111">Otevřete centrum pro správu Exchange.</span><span class="sxs-lookup"><span data-stu-id="78979-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="78979-112">Klikněte na **organizace**a potom poklikejte na zásadu přiřazenou uživateli v části **individuální sdílení**.</span><span class="sxs-lookup"><span data-stu-id="78979-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="78979-113">Toto je zásada vrácená v kroku 2.</span><span class="sxs-lookup"><span data-stu-id="78979-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="78979-114">Na stránce pravidlo sdílení vyberte úroveň sdílení kalendáře, kterou chcete povolit v části **Určete, jaké informace chcete sdílet**. klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="78979-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="78979-115">Další informace najdete v tématu: ["zásady neumožňují udělit oprávnění na této úrovni jednomu nebo více příjemcům při pokusu o sdílení kalendáře uživatelem](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="78979-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
