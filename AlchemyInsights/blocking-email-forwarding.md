---
title: Blokování nebo odblokování externího automatického přeposílání e-mailů
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315867"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokování nebo odblokování věčných automatických přeposílání e-mailů

Pokud chcete povolit nebo zakázat přeposílání e-mailů pro určitou poštovní schránku, podívejte se na tématu [Konfigurace přesměrování e-mailů](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Správci mohou řídit externí přeposílání pro organizaci pomocí [zásad odchozích spamů](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy). Zásady odchozího spamu můžete spravovat na Microsoft 365 Defender nebo pomocí rutiny <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) v Exchange Online PowerShellu.

Pokud se zobrazí následující chybová zpráva: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access denied, Your organization does not allow external forwarding) (550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access denied, Your organization does not allow external forwarding) (550 5.7.520 Access denied, Your organization does not allow external forwardinging) (550 5.**

**Poznámka:** Doporučujeme výchozí hodnotu Automaticky **–**  systém řízený pro nastavení pravidel automatického přeposílání ve vaší výchozí zásadách filtru odchozích spamů (automatické externí přeposílání je zablokované, interní automatické přeposílání stále funguje). Měli byste vytvořit vlastní zásady filtru odchozích spamů a použít hodnotu **Zapnuto –** Přeposílání je povolené jenom pro uživatele, kteří potřebují externí automatické přeposílání e-mailů. Další informace najdete v tématu [Konfigurace externího přeposílání e-mailů v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
