---
title: Používání DLP v pravidlech přenosu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827209"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="eef56-102">Používání DLP v pravidlech přenosu</span><span class="sxs-lookup"><span data-stu-id="eef56-102">Using DLP in transport rules</span></span>

<span data-ttu-id="eef56-103">Pokud chcete do existujícího přenosu integrovat ochranu před únikem informací (DLP), v nastavení pravidla přenosu použijte podmínku „**Pokud zpráva obsahuje… citlivé informace**“.</span><span class="sxs-lookup"><span data-stu-id="eef56-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="eef56-104">**Podrobnosti viz:**</span><span class="sxs-lookup"><span data-stu-id="eef56-104">**For more details, see:**</span></span>

- <span data-ttu-id="eef56-105">Typy citlivých informací integrované DLP v pravidlech přenosu: [Integrace pravidel pro citlivé informace](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="eef56-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="eef56-106">Pravidlo také můžete otestovat pomocí testovacího režimu, a to s testem zásad, nebo bez něj.</span><span class="sxs-lookup"><span data-stu-id="eef56-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="eef56-107">Než nově vytvořené pravidlo otestujete, musíte počkat 30 minut.</span><span class="sxs-lookup"><span data-stu-id="eef56-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="eef56-108">Viz článek [Testování pravidel toku pošty / přenosu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).</span><span class="sxs-lookup"><span data-stu-id="eef56-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="eef56-109">**Poznámka**: Pokud se pro pravidla přenosu v EAC pokoušíte zavést novou zásadu DLP, použijte místo toho [Zásady DLC v Centru zabezpečení a dodržování předpisů](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="eef56-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
