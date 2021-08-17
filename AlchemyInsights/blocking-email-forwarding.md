---
title: 726 Blokování přeposílání e-mailů
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059625"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokování nebo odblokování přeposílání e-mailů

Pokud chcete povolit nebo zakázat přeposílání e-mailů pro určitou poštovní schránku, podívejte se na informace v [tématu Konfigurace přesměrování e-mailů.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Na úrovni tenanta se řízení externího přeposílání provádí pomocí zásad odchozích spamů. Zásady filtru odchozích spamů můžete zkontrolovat [](https://protection.office.com/antispam) tady v Centru zabezpečení a dodržování předpisů nebo pomocí příkazu [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Pokud se zobrazí následující chybová zpráva: **"550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access denied, Your organization does not allow external forwarding) (550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7.520 Access denied, Your organization does not allow external forwarding) (550 5.7.520 Access denied, Your organization does not allow external forwarding" (550 5.7**

**Poznámka:** U výchozích zásad filtru odchozích spamů se doporučuje zakázat externí automatické přeposílání a povolit ho jenom uživatelům, kteří potřebují externí přeposílání, a to tak, že pro tyto uživatele vytvoříte vlastní zásadu. Další informace najdete v tématu [Konfigurace externího přeposílání e-mailů v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).