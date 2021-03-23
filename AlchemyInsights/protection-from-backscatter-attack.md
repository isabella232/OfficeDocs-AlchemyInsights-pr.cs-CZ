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
# <a name="protection-from-backscatter-attack"></a>Ochrana před útokem backscatteru

Backscatter je oznámení o nedoručení (označované taky jako oznámení o nedoručení nebo zprávy o nedoručování zpráv), které dostáváte pro zprávy, které jste neposílal(a). Spammers forge (spoof) **the From: address** of their messages, and they often use real email addresses to lend credibility to their messages. Takže když odesílatelé nevyžádané pošty nevyhnutelně pošlou zprávy neexistující příjemcům, cílový e-mailový server je v podstatě záludný k vrácení nedoručitelné zprávy v oznámení o nedoručení kované odesílateli v **adrese Od:.**

Další informace najdete v části [Backscatter v EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Povolení ochrany backscatterem**

Pokud chcete zapnout ochranu backscatteru, postupujte podle následující cesty.

**protection.office.com > Zásady správy hrozeb > > Antispam > Vyberte zásady filtru spamu > Upravit zásady > Vlastnosti spamu > Označit jako spam > NDR backscatter > Nastavit ho na "On"**

Pokud se domníváte, že byl účet ohrožený, podívejte se na toto:

- [Odpovídání na ohrožený e-mailový účet](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Odebrání blokovaných uživatelů z portálu Uživatelé s omezeným přístupem v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



