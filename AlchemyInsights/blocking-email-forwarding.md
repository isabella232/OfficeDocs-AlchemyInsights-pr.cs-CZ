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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473094"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="10ffb-102">Blokování nebo zrušení blokování přeposílání e-mailů</span><span class="sxs-lookup"><span data-stu-id="10ffb-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="10ffb-103">Informace o povolení nebo zakázání předávání [e-](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)mailů pro konkrétní poštovní schránku</span><span class="sxs-lookup"><span data-stu-id="10ffb-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="10ffb-104">Na úrovni tenanta je kontrola externího předávání dokončena pomocí zásad odchozích spamů.</span><span class="sxs-lookup"><span data-stu-id="10ffb-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="10ffb-105">Zásady odchozí nevyžádané zprávy můžete zkontrolovat v centru zabezpečení a dodržování předpisů [tady] ( https://protection.office.com/antispam) nebo pomocí [příkazu Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="10ffb-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="10ffb-106">Pokud se zobrazí tato chybová zpráva: **"550 5.7.520 Access denied, vaše organizace neumožňuje externí předávání"**, ujistěte se, že je zásada nakonfigurovaná tak, aby umožňovala externí Automatický přesun.</span><span class="sxs-lookup"><span data-stu-id="10ffb-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="10ffb-107">**Poznámka:** Doporučujeme, aby byl externí Automatický přepočet vypnutý ve výchozích zásadách odchozích e-mailových filtrů nevyžádané pošty, a povolit ho jenom pro uživatele, kteří potřebují externí předávání, a to tak, že si pro tyto uživatele vytvoří vlastní zásadu.</span><span class="sxs-lookup"><span data-stu-id="10ffb-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="10ffb-108">Další informace najdete v článku [konfigurace předávání externích e-mailů v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="10ffb-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>