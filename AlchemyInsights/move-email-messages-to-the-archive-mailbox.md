---
title: Přesunutí e-mailových zpráv do poštovní schránky Archivu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522764"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="e87c5-102">Přesunutí e-mailu do archivní poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="e87c5-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="e87c5-103">Pokud chcete, abychom spouštěli automatické kontroly níže uvedených nastavení, vyberte tlačítko Zpět < v horní části této stránky a zadejte e-mailovou adresu uživatele, který má problémy s přesunem e-mailu do své archivní schránky.</span><span class="sxs-lookup"><span data-stu-id="e87c5-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="e87c5-104">Zkontrolujte, zda byla povolena **poštovní schránka Archivu.**</span><span class="sxs-lookup"><span data-stu-id="e87c5-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="e87c5-105">Pokud ne, použijte kroky v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) povolit archivní poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="e87c5-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="e87c5-106">Chcete-li automaticky archivovat zprávy do archivní poštovní schránky, musí být značka uchovávání informací s akcí **Přesunout do archivace** nastavena tak, **aby se automaticky použila na značku celé poštovní schránky (výchozí).**</span><span class="sxs-lookup"><span data-stu-id="e87c5-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="e87c5-107">Pomocí pokynů vytvořte značku: [Archivovat výchozí značku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="e87c5-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="e87c5-108">Dále přidejte značku **Archiv** do zásad uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="e87c5-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="e87c5-109">V Centru pro správu Exchange zvolte **Zásady uchovávání informací** > přidat **značku Přesunout do archivace** do zásady > **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="e87c5-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="e87c5-110">Nyní [přiřaďte zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovní schránce konkrétního uživatele.</span><span class="sxs-lookup"><span data-stu-id="e87c5-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="e87c5-111">Stejné zásady budou použity pro **primární** i **archivní** poštovní schránku.</span><span class="sxs-lookup"><span data-stu-id="e87c5-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="e87c5-112">Může být nutné vynutit spuštění Pomocníka pro spravované složky (MFA) a použít nové nastavení poštovní schránky uživatele.</span><span class="sxs-lookup"><span data-stu-id="e87c5-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="e87c5-113">Spuštěním následujícího příkazu při [připojení k EXO PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spusťte Pomocníka pro spravované složky pro určitou poštovní schránku:</span><span class="sxs-lookup"><span data-stu-id="e87c5-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="e87c5-114">Start-ManagedFolderAssistant -Identita<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="e87c5-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="e87c5-115">Další informace o nastavení zásad archivace naleznete v [tématu Nastavení zásad archivace a odstranění poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="e87c5-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  