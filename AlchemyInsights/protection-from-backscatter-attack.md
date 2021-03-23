---
title: Ochrana před útokem backscatteru
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035078"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="9e2a5-102">Ochrana před útokem backscatteru</span><span class="sxs-lookup"><span data-stu-id="9e2a5-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="9e2a5-103">Backscatter je oznámení o nedoručení (označované taky jako oznámení o nedoručení nebo zprávy o nedoručování zpráv), které dostáváte pro zprávy, které jste neposílal(a).</span><span class="sxs-lookup"><span data-stu-id="9e2a5-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="9e2a5-104">Spammers forge (spoof) **the From: address** of their messages, and they often use real email addresses to lend credibility to their messages.</span><span class="sxs-lookup"><span data-stu-id="9e2a5-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="9e2a5-105">Takže když odesílatelé nevyžádané pošty nevyhnutelně pošlou zprávy neexistující příjemcům, cílový e-mailový server je v podstatě záludný k vrácení nedoručitelné zprávy v oznámení o nedoručení kované odesílateli v **adrese Od:.**</span><span class="sxs-lookup"><span data-stu-id="9e2a5-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="9e2a5-106">Další informace najdete v části [Backscatter v EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="9e2a5-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="9e2a5-107">**Povolení ochrany backscatterem**</span><span class="sxs-lookup"><span data-stu-id="9e2a5-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="9e2a5-108">Pokud chcete zapnout ochranu backscatteru, postupujte podle následující cesty.</span><span class="sxs-lookup"><span data-stu-id="9e2a5-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="9e2a5-109">**protection.office.com > Zásady správy hrozeb > > Antispam > Vyberte zásady filtru spamu > Upravit zásady > Vlastnosti spamu > Označit jako spam > NDR backscatter > Nastavit ho na "On"**</span><span class="sxs-lookup"><span data-stu-id="9e2a5-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="9e2a5-110">Pokud se domníváte, že byl účet ohrožený, podívejte se na toto:</span><span class="sxs-lookup"><span data-stu-id="9e2a5-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="9e2a5-111">Odpovídání na ohrožený e-mailový účet</span><span class="sxs-lookup"><span data-stu-id="9e2a5-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="9e2a5-112">Odebrání blokovaných uživatelů z portálu Uživatelé s omezeným přístupem v Office 365</span><span class="sxs-lookup"><span data-stu-id="9e2a5-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



