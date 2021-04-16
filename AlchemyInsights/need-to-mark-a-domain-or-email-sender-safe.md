---
title: Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792125"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="4bf90-102">Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?</span><span class="sxs-lookup"><span data-stu-id="4bf90-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="4bf90-103">Použití seznamů **bezpečných odesílatelů se nedoporučuje,** protože se ve vaší organizaci otevírá útoky spamu, phish a falšování falšování.</span><span class="sxs-lookup"><span data-stu-id="4bf90-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="4bf90-104">Pokud ale existuje obchodní požadavek, doporučujeme **k** tomu použít pravidla **[toku](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pošty.</span><span class="sxs-lookup"><span data-stu-id="4bf90-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="4bf90-105">Naše pokyny zajistí ověření odesílatele (ověření, že se doména odesílání neschová).</span><span class="sxs-lookup"><span data-stu-id="4bf90-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="4bf90-106">**Poznámka:** Nedoporučujeme spravovat falešná pozitiva pomocí seznamů bezpečných odesílatelů, protože výjimky z filtrování spamu mohou otevřít vaši organizaci kvůli útokům zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="4bf90-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="4bf90-107">Pokud vaši uživatel(é) dostávají zprávy nesprávně označené jako spam nebo nevyžádané e-maily, nahlásit zprávy a **[soubory microsoftu](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="4bf90-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="4bf90-108">Je třeba se vyhnout bezpečným odesílatelům v Outlooku, seznamu povolených odesílatelů nebo seznamu povolených domén v zásadách ochrany proti spamu, protože odesílatelé obcházejí veškerý spam, falšování identity a phish ochranu a ověřování odesílatele (SPF, DKIM, DMARC). </span><span class="sxs-lookup"><span data-stu-id="4bf90-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="4bf90-109">Tato metoda se nejlépe používá jenom pro dočasné testování.</span><span class="sxs-lookup"><span data-stu-id="4bf90-109">This method is best used for temporary testing only.</span></span>
