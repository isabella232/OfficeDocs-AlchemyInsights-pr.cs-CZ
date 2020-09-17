---
title: Přesunutí e-mailových zpráv do archivní poštovní schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799773"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="54a77-102">Přesunutí e-mailu do archivní poštovní schránky</span><span class="sxs-lookup"><span data-stu-id="54a77-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="54a77-103">Pokud chcete, abychom mohli spustit automatizované kontroly pro níže uvedené nastavení, klikněte na tlačítko zpět <--v horní části této stránky zadejte e-mailovou adresu uživatele, který má problémy s přesunutím e-mailu do archivované poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="54a77-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="54a77-104">Zkontrolujte, že je povolená **poštovní schránka** .</span><span class="sxs-lookup"><span data-stu-id="54a77-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="54a77-105">Pokud ne, povolte archivaci poštovní schránky podle pokynů v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) .</span><span class="sxs-lookup"><span data-stu-id="54a77-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="54a77-106">Pokud chcete, aby se zprávy automaticky archivoval do archivní poštovní schránky, musí být nastavena značka pro uchování informací, která **se má** **automaticky použít u celé značky poštovní schránky (výchozí)**.</span><span class="sxs-lookup"><span data-stu-id="54a77-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="54a77-107">Postupujte podle pokynů pro vytvoření značky: [výchozí nastavení archivu](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="54a77-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="54a77-108">Potom **přidejte do zásad** uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="54a77-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="54a77-109">V centru pro správu Exchange zvolte **zásady uchovávání informací** , > přidejte **značku pro přesunutí do** složky > **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="54a77-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="54a77-110">Teď [přiřaďte zásady uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovní schránce určitého uživatele.</span><span class="sxs-lookup"><span data-stu-id="54a77-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="54a77-111">Stejné zásady se uplatní pro poštovní schránku **hlavní** i **archiv** .</span><span class="sxs-lookup"><span data-stu-id="54a77-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="54a77-112">Může být nutné vynutit spuštění pomocníka pro správu složek (MFA) a použít nové nastavení u poštovní schránky uživatele.</span><span class="sxs-lookup"><span data-stu-id="54a77-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="54a77-113">Spuštěním tohoto příkazu po [připojení k EXO PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustíte Pomocníka pro správu složky pro konkrétní poštovní schránku:</span><span class="sxs-lookup"><span data-stu-id="54a77-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="54a77-114">Start-ManagedFolderAssistant-identita <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="54a77-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="54a77-115">Další informace o nastavení zásad archivace najdete v tématu [nastavení zásad archivace a odstraňování poštovních schránek](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="54a77-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  