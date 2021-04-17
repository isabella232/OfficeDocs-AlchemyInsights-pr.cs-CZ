---
title: Vytvoření e-mailu zachyťte vše
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816193"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="39425-102">Vytvoření e-mailu zachyťte vše</span><span class="sxs-lookup"><span data-stu-id="39425-102">Create an email catch all</span></span>

<span data-ttu-id="39425-103">Použití všech úlovek se důrazně nedoporučuje.</span><span class="sxs-lookup"><span data-stu-id="39425-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="39425-104">Je lepší vrátit odesílateli zprávu, která odesílatelům umožní zjistit, že jejich zprávu nelze doručit jako adresu, aby mohli provést akci.</span><span class="sxs-lookup"><span data-stu-id="39425-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="39425-105">Monitorovanou poštovní schránku můžete omezit jenom na zachycení dříve platných e-mailových adres.</span><span class="sxs-lookup"><span data-stu-id="39425-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="39425-106">Každá poštovní schránka, která zachytí všechny poštovní schránky, dostane hodně spamu a může se vyplnit, pokud není pečlivě sledována.</span><span class="sxs-lookup"><span data-stu-id="39425-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="39425-107">(Existují limity příjmu.)</span><span class="sxs-lookup"><span data-stu-id="39425-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="39425-108">Pokud se rozhodnete pokračovat, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="39425-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="39425-109">Vytvořte dynamickou distribuční skupinu, & "Všechny typy příjemců".</span><span class="sxs-lookup"><span data-stu-id="39425-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="39425-110">Vytvořte vyhrazenou poštovní schránku pro zachycení e-mailů, například catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="39425-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="39425-111">Pro konkrétní doménu nastavte Typ_domény na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="39425-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="39425-112">Pokud později odeberete všechny zachytáky, nezapomeňte doménu nastavit zpátky na Autoritativní.</span><span class="sxs-lookup"><span data-stu-id="39425-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="39425-113">Vytvořte pravidlo přenosu pošty takto:</span><span class="sxs-lookup"><span data-stu-id="39425-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="39425-114">Pokud je odesílatel mimo organizaci</span><span class="sxs-lookup"><span data-stu-id="39425-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="39425-115">Přesměrovat zprávu na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="39425-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="39425-116">S výjimkou případu, kdy je příjemce členem allusers@domain.com (distribuční skupina obsahuje všechny členy)</span><span class="sxs-lookup"><span data-stu-id="39425-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="39425-117">Ujistěte se, že se nové poštovní schránky přidávají do dynamické distribuční skupiny.</span><span class="sxs-lookup"><span data-stu-id="39425-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
