---
title: 1336 RecoverableItems je plná.
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741260"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="d7e1a-102">Složka pro obnovitelnou položky je plná</span><span class="sxs-lookup"><span data-stu-id="d7e1a-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="d7e1a-103">U poštovních schránek Exchange Online je výchozí limit úložiště pro složku pro obnovitelnost položek 30 GB.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="d7e1a-104">Pokud je poštovní schránka umístěná na podržení soudního sporu, podržení eDiscovery nebo je přiřazená zásada uchovávání informací, automaticky se 100 zvýší limit úložiště pro složku pro obnovitelnou položky.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="d7e1a-105">Když složka se obnovitelnou položkami dosáhne limitu úložiště, bude funkčnost poštovní schránky ovlivněna následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="d7e1a-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="d7e1a-106">Uživatel nemůže odstranit položky z poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="d7e1a-107">Pomocník pro spravovanou složku nemůže odstranit položky na základě značky uchovávání informací nebo nastavení spravované složky.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="d7e1a-108">U poštovních schránek, které mají povoleno obnovení jedné položky nebo jsou blokovány, nedokáže proces ochrany stránky kopírováním na disk zachovat verze položek upravovaných uživatelem.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="d7e1a-109">V případě poštovních schránek s povoleným protokolováním auditu poštovní schránky nelze do podsložky prověřit položky ukládat žádné položky protokolu auditování poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="d7e1a-110">U poštovních schránek, které nejsou blokovány, můžou správci pomocí `Search-Mailbox -SearchDumpsterOnly -DeleteContent` příkazu v PowerShellu pro Exchange Online odstranit položky ve složce obnovitelnou položky.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="d7e1a-111">Další informace najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="d7e1a-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="d7e1a-112">Hledání a odstraňování zpráv</span><span class="sxs-lookup"><span data-stu-id="d7e1a-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="d7e1a-113">Hledání – poštovní schránka</span><span class="sxs-lookup"><span data-stu-id="d7e1a-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="d7e1a-114">U poštovních schránek, které jsou blokovány, musí správci odebrat držení před odstraněním položek ze složky pro obnovitelnou položky.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="d7e1a-115">Další informace najdete v článku [o blokování položek ve složce pro obnovitelnou položky v cloudových poštovních schránkách](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="d7e1a-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="d7e1a-116">Aby se zabránilo tomu, že se složka pro obnovu položek zablokuje, můžou správci zvýšit limit úložiště složky prohledatelné položky pro blokované poštovní schránky a nastavit zásady uchovávání poštovní schránky, které přesunou položky ze složky prohledatelné položky do archivované poštovní schránky uživatele.</span><span class="sxs-lookup"><span data-stu-id="d7e1a-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="d7e1a-117">Přečtěte si téma [zvýšení kvóty pro obnovitelnou položky pro blokované poštovní schránky](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="d7e1a-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
