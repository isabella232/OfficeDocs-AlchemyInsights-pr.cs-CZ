---
title: Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803238"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="f625a-102">Potřebujete označit doménu nebo odesílatele e-mailu jako bezpečné?</span><span class="sxs-lookup"><span data-stu-id="f625a-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="f625a-103">Používání **seznamů bezpečných odesílatelů se nedoporučuje** , protože otevře vaši organizaci útoky spamu, phishingu a falšování identity.</span><span class="sxs-lookup"><span data-stu-id="f625a-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="f625a-104">Pokud je ale požadován podnik, **doporučujeme použít pro** toto **[pravidlo toku pošty](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="f625a-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="f625a-105">Naše pokyny zajistí ověření odesílatele (ověřuje, jestli není zafalešnovaná doména).</span><span class="sxs-lookup"><span data-stu-id="f625a-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="f625a-106">**Poznámka**: Nedoporučujeme správu falešných falešných zpráv pomocí seznamů bezpečných odesílatelů, protože výjimky pro filtrování spamu můžou vaši organizaci otevřít na útoky zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="f625a-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="f625a-107">Pokud vaše uživatelé neoznačili zprávy nesprávně označené jako spam nebo Nevyžádaná pošta, **[ohlaste jim zprávy a soubory Microsoftu](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="f625a-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="f625a-108">Bezpeční odesílatelé v Outlooku, seznamu povolených odesílatelů nebo seznam povolených domén v zásadách ochrany před nevyžádanou poštou **by měli být zabráněno** , protože odesílatelé vycházejí ze všech spamů, falešných zpráv a ochrany proti podvodné poště (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="f625a-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="f625a-109">Tento způsob je nejvhodnější pro dočasné testování.</span><span class="sxs-lookup"><span data-stu-id="f625a-109">This method is best used for temporary testing only.</span></span>
