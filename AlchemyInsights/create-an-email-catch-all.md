---
title: Vytvoření veškerého e-mailového catch
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712979"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="f2a93-102">Vytvoření veškerého e-mailového catch</span><span class="sxs-lookup"><span data-stu-id="f2a93-102">Create an email catch all</span></span>

<span data-ttu-id="f2a93-103">Důrazně se nedoporučuje použít veškerý úlovek.</span><span class="sxs-lookup"><span data-stu-id="f2a93-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="f2a93-104">Je lepší poskytnout odesilateli zpátky, kteří mu odešlou vědět, že nemohly být doručeny, aby mohli dělat žádné kroky.</span><span class="sxs-lookup"><span data-stu-id="f2a93-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="f2a93-105">Sledovanou poštovní schránku můžete také omezit tak, aby bylo možné zachytit dříve platné e-mailové adresy.</span><span class="sxs-lookup"><span data-stu-id="f2a93-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="f2a93-106">Všechny úlovky budou dostávat dobré věci nevyžádané pošty a mohou nakonec plnit případné Nesledované.</span><span class="sxs-lookup"><span data-stu-id="f2a93-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="f2a93-107">(Existují limity.)</span><span class="sxs-lookup"><span data-stu-id="f2a93-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="f2a93-108">Pokud se rozhodnete pokračovat, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="f2a93-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="f2a93-109">Vytvořte dynamickou distribuční skupinu & zahrnout "všechny typy příjemců".</span><span class="sxs-lookup"><span data-stu-id="f2a93-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="f2a93-110">Vytvořte vyhrazenou poštovní schránku pro zachycování e-mailů, například catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="f2a93-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="f2a93-111">Pro určitou doménu nastavte DomainType na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="f2a93-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="f2a93-112">Pokud později zachytíte celý úlovek, nastavte doménu zpět na hodnotu autoritativní.</span><span class="sxs-lookup"><span data-stu-id="f2a93-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="f2a93-113">Vytvořte – Poštyhttps://Configure.Office.com/Scenario.aspx?SID=12:</span><span class="sxs-lookup"><span data-stu-id="f2a93-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="f2a93-114">Pokud je odesílatel "mimo organizaci"</span><span class="sxs-lookup"><span data-stu-id="f2a93-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="f2a93-115">Přesměrovat zprávu na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="f2a93-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="f2a93-116">Kromě případu, kdy je příjemce členem allusers@domain.com (distribuční skupina obsahuje všechny členy)</span><span class="sxs-lookup"><span data-stu-id="f2a93-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="f2a93-117">Ověření, že nové poštovní schránky se přidají do dynamické distribuční skupiny</span><span class="sxs-lookup"><span data-stu-id="f2a93-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
