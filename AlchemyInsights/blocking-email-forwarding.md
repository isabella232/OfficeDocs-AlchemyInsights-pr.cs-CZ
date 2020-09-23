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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219848"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokování nebo zrušení blokování přeposílání e-mailů

Informace o povolení nebo zakázání předávání [e-](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)mailů pro konkrétní poštovní schránku

Na úrovni klienta je kontrola externího předávání provedená pomocí zásad odchozích spamů. Pokud je tato možnost vypnutá nebo automatická, může blokovat přeposílání e-mailů pomocí "550 5.7.520 Access denied, ale vaše organizace neumožňuje chybu externího předávání. V případě, že je předávání nastaveno jako blokované, to je chyba, kterou uživatelé uvidí.

Pokud zablokujete přesměrování, ujistěte se, že je zásada nakonfigurovaná tak, aby umožňovala externí přesměrování. Zásady odchozí nevyžádané zprávy můžete zkontrolovat v centru zabezpečení a dodržování předpisů nebo pomocí příkazu Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode. Pokud chcete nastavit blokování pro přeposílání zpráv, je stejný příkaz shodný se stavem zásad.

Poznámka: doporučuje se, aby byl externí Automatický přepočet vypnutý ve výchozích zásadách odchozích Spamních filtrů a povolil se mu jenom pro uživatele, kteří potřebují externí předávání, a to tak, že pro tyto uživatele vytvoří vlastní zásadu. Další informace najdete v článku [konfigurace předávání externích e-mailů v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).