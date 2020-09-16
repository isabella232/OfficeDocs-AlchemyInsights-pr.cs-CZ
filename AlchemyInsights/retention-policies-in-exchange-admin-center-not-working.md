---
title: Zásady uchovávání informací v centru pro správu Exchange nefungují
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740503"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="69a44-102">Zásady uchovávání informací v centru pro správu Exchange</span><span class="sxs-lookup"><span data-stu-id="69a44-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="69a44-103">Pokud chcete, abychom mohli spustit automatizované kontroly pro níže uvedené nastavení, klikněte na tlačítko zpět <--v horní části této stránky zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="69a44-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="69a44-104">**Problém:** Nově vytvořené nebo aktualizované zásady uchovávání informací v centru pro správu Exchange se nevztahují na poštovní schránky ani položky, které se nepřesunou, ani se neodstraní.</span><span class="sxs-lookup"><span data-stu-id="69a44-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="69a44-105">**Hlavní příčiny:**</span><span class="sxs-lookup"><span data-stu-id="69a44-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="69a44-106">Příčinou může být to, že **Pomocník pro spravovanou složku** nezpracoval poštovní schránku uživatele.</span><span class="sxs-lookup"><span data-stu-id="69a44-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="69a44-107">Pomocník pro spravovanou složku se pokusí zpracovat každou poštovní schránku v cloudové organizaci každých 7 dní.</span><span class="sxs-lookup"><span data-stu-id="69a44-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="69a44-108">Pokud změníte značku uchovávání informací nebo použijete jiné zásady uchovávání informací pro poštovní schránku, můžete počkat, dokud se spravovaná složka nepomůže zpracovávat, nebo spusťte rutinu Start-ManagedFolderAssistant, abyste mohli spustit konkrétní poštovní schránku.</span><span class="sxs-lookup"><span data-stu-id="69a44-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="69a44-109">Tato rutina je užitečná pro účely testování nebo odstraňování potíží s nastavením zásad uchovávání informací nebo nastavení značek uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="69a44-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="69a44-110">Další informace najdete v [části spuštění pomocníka pro správu složek](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="69a44-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="69a44-111">**Řešení:** Spuštěním následujícího příkazu spustíte Pomocníka pro správu složky pro konkrétní poštovní schránku:</span><span class="sxs-lookup"><span data-stu-id="69a44-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="69a44-112">Může k tomu dojít také v případě, že je na poštovní schránce **povolený** **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="69a44-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="69a44-113">Pokud byla poštovní schránka umístěna na RetentionHold, nebudou zásady uchovávání informací v poštovní schránce během této doby zpracovány.</span><span class="sxs-lookup"><span data-stu-id="69a44-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="69a44-114">Další Informaton o nastavení RetentionHold najdete v tématu: [blokování zadržení poštovní schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="69a44-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="69a44-115">**Průzkumníku**</span><span class="sxs-lookup"><span data-stu-id="69a44-115">**Solution:**</span></span>
    
  - <span data-ttu-id="69a44-116">Zkontrolujte stav nastavení RetentionHold pro určitou poštovní schránku v [EXO PowerShellu](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="69a44-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="69a44-117">Spuštěním následujícího příkazu **zakážete** RetentionHold v konkrétní poštovní schránce:</span><span class="sxs-lookup"><span data-stu-id="69a44-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="69a44-118">Spusťte znovu pomocníka Správa složek:</span><span class="sxs-lookup"><span data-stu-id="69a44-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="69a44-119">**Poznámka:** Pokud je poštovní schránka menší než 10 MB, nebude poštovní schránka automaticky zpracovávat Pomocník pro správu složek.</span><span class="sxs-lookup"><span data-stu-id="69a44-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="69a44-120">Další informace o zásadách uchovávání informací v centru pro správu Exchange najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="69a44-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="69a44-121">Značky a zásady uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="69a44-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="69a44-122">Použití zásad uchovávání informací u poštovních schránek</span><span class="sxs-lookup"><span data-stu-id="69a44-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="69a44-123">Přidání nebo odebrání značek uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="69a44-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="69a44-124">Jak zjistit typ blokování na poštovní schránce</span><span class="sxs-lookup"><span data-stu-id="69a44-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
