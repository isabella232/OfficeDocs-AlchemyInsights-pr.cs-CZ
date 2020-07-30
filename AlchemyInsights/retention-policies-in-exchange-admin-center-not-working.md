---
title: Zásady uchovávání informací v Centru pro správu Exchange nefungují
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522800"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="8a494-102">Zásady uchovávání informací v Centru pro správu Exchange</span><span class="sxs-lookup"><span data-stu-id="8a494-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="8a494-103">Pokud chcete, abychom spouštěli automatické kontroly níže uvedených nastavení, vyberte v horní části této stránky tlačítko Zpět < a zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="8a494-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="8a494-104">**Problém:** Nově vytvořené nebo aktualizované zásady uchovávání informací v Centru pro správu Exchange se nevztahují na poštovní schránky nebo položky nejsou přesunuty do poštovní schránky archivu nebo odstraněny.</span><span class="sxs-lookup"><span data-stu-id="8a494-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="8a494-105">**Příčiny:**</span><span class="sxs-lookup"><span data-stu-id="8a494-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="8a494-106">Důvodem může být, že **Pomocník pro spravované složky** nezpracoval poštovní schránku uživatele.</span><span class="sxs-lookup"><span data-stu-id="8a494-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="8a494-107">Pomocník pro spravované složky se pokusí zpracovat každou poštovní schránku v organizaci na principu shluků jednou za sedm dní.</span><span class="sxs-lookup"><span data-stu-id="8a494-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="8a494-108">Pokud změníte značku uchovávání informací nebo použijete jinou zásadu uchovávání informací pro poštovní schránku, můžete počkat, dokud pomoc s spravované složky zpracuje poštovní schránku, nebo můžete spustit rutinu Start-ManagedFolderAssistant a spustit Pomocníka pro spravované složky ke zpracování konkrétní poštovní schránky.</span><span class="sxs-lookup"><span data-stu-id="8a494-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="8a494-109">Spuštění této rutiny je užitečné pro testování nebo řešení potíží se zásadami uchovávání informací nebo nastavením značky uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="8a494-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="8a494-110">Další informace naleznete na stránce [Spuštění Pomocníka pro spravované složky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="8a494-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="8a494-111">**Řešení:** Spuštěním následujícího příkazu spusťte Pomocníka pro spravované složky pro určitou poštovní schránku:</span><span class="sxs-lookup"><span data-stu-id="8a494-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="8a494-112">K tomu může dojít také v **případě, že retentionhold** byla **povolena** v poštovní schránce.</span><span class="sxs-lookup"><span data-stu-id="8a494-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="8a494-113">Pokud poštovní schránka byla umístěna na RetentionHold, zásady uchovávání informací v poštovní schránce nebudou zpracovány během této doby.</span><span class="sxs-lookup"><span data-stu-id="8a494-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="8a494-114">Další informace o nastavení retentionhold najdete v tématu: [Blokování uchovávání poštovní schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="8a494-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="8a494-115">**Řešení:**</span><span class="sxs-lookup"><span data-stu-id="8a494-115">**Solution:**</span></span>
    
  - <span data-ttu-id="8a494-116">Zkontrolujte stav nastavení RetentionHold na konkrétní poštovní schránce v [prostředí EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="8a494-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="8a494-117">Spuštěním následujícího příkazu **zakázat** RetentionHold na konkrétní poštovní schránky:</span><span class="sxs-lookup"><span data-stu-id="8a494-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="8a494-118">Nyní znovu spusťte Pomocníka pro spravované složky:</span><span class="sxs-lookup"><span data-stu-id="8a494-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="8a494-119">**Poznámka:** Pokud je poštovní schránka menší než 10 MB, Pomocník pro spravované složky poštovní schránku automaticky nezpracuje.</span><span class="sxs-lookup"><span data-stu-id="8a494-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="8a494-120">Další informace o zásadách uchovávání informací v Centru pro správu Exchange najdete v následujících tématech:</span><span class="sxs-lookup"><span data-stu-id="8a494-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="8a494-121">Značky uchovávání informací a zásady uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="8a494-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="8a494-122">Použití zásad uchovávání informací u poštovních schránek</span><span class="sxs-lookup"><span data-stu-id="8a494-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="8a494-123">Přidání nebo odebrání značek uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="8a494-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="8a494-124">Jak identifikovat typ blokování umístěného v poštovní schránce</span><span class="sxs-lookup"><span data-stu-id="8a494-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
