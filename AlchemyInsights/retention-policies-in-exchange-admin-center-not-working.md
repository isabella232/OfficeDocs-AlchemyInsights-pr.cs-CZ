---
title: Zásady uchovávání informací v Centru pro správu Exchange nefungují
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952221"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9fb9a-102">Zásady uchovávání informací v Centru pro správu Exchange</span><span class="sxs-lookup"><span data-stu-id="9fb9a-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="9fb9a-103">Pokud chcete, abychom spouštěli automatické kontroly nastavení uvedených níže, vyberte tlačítko Zpět <– v horní části této stránky a potom zadejte e-mailovou adresu uživatele, který má problémy se zásadami uchovávání informací.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="9fb9a-104">Pokud máte problémy se zásadami uchovávání informací v Centru pro správu Exchange, které se neakusují u poštovních schránek nebo položek, které se do archivační poštovní schránky přesouvá, zkontrolujte toto:</span><span class="sxs-lookup"><span data-stu-id="9fb9a-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="9fb9a-105">**Hlavní příčiny:**</span><span class="sxs-lookup"><span data-stu-id="9fb9a-105">**Root Causes:**</span></span>

- <span data-ttu-id="9fb9a-106">**Pomocník pro spravované** složky nezpracuje poštovní schránku uživatele.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="9fb9a-107">Pomocník pro spravované složky se pokusí zpracovat každou poštovní schránku ve vaší cloudové organizaci jednou za sedm dní.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="9fb9a-108">**Řešení:** Spusťte Pomocníka pro spravované složky.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="9fb9a-109">**Funkce RetentionHold** je **v** poštovní schránce povolená.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="9fb9a-110">Pokud je poštovní schránka umístěná na zadržovací držaně, zásady uchovávání informací v poštovní schránce se během této doby nezpracují.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="9fb9a-111">**Řešení:** Zkontrolujte stav nastavení uchovávání informací a podle potřeby aktualizujte.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="9fb9a-112">Podrobnosti najdete v tématu [Blokování uchovávání poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="9fb9a-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="9fb9a-113">**Poznámka:** Pokud je poštovní schránka menší než 10 MB, Pomocník pro spravované složky poštovní schránku automaticky nezpracuje.</span><span class="sxs-lookup"><span data-stu-id="9fb9a-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="9fb9a-114">Další informace o zásadách uchovávání informací v Centru pro správu Exchange najdete v tématu:</span><span class="sxs-lookup"><span data-stu-id="9fb9a-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="9fb9a-115">Značky uchovávání informací a zásady uchovávání informací</span><span class="sxs-lookup"><span data-stu-id="9fb9a-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="9fb9a-116">[Použití zásad uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nebo [přidání nebo odebrání značek uchovávání informací](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="9fb9a-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="9fb9a-117">Jak identifikovat typ blokování umístěného v poštovní schránce</span><span class="sxs-lookup"><span data-stu-id="9fb9a-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
