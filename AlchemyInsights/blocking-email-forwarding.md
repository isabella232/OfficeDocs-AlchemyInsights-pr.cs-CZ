---
title: 726 blokování přeposlání e-mailu
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478319"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokování nebo zrušení blokování přeposílání e-mailů

Informace o povolení nebo zakázání předávání [e-](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)mailů pro konkrétní poštovní schránku

Na úrovni tenanta je kontrola externího předávání dokončena pomocí zásad odchozích spamů. Zásady odchozí nevyžádané pošty v centru zabezpečení a dodržování předpisů můžete zkontrolovat [tady](https://protection.office.com/antispam) nebo pomocí [příkazu Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Pokud se zobrazí tato chybová zpráva: **"550 5.7.520 Access denied, vaše organizace neumožňuje externí předávání"**, ujistěte se, že je zásada nakonfigurovaná tak, aby umožňovala externí Automatický přesun.

**Poznámka:** Doporučujeme, aby byl externí Automatický přepočet vypnutý ve výchozích zásadách odchozích e-mailových filtrů nevyžádané pošty, a povolit ho jenom pro uživatele, kteří potřebují externí předávání, a to tak, že si pro tyto uživatele vytvoří vlastní zásadu. Další informace najdete v článku [konfigurace předávání externích e-mailů v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).