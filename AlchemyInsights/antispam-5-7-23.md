---
title: Antispam – 5,7,23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821404"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="89217-102">Řešení problémů s doručováním e-mailů s kódem chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="89217-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="89217-103">Ověřte záznam DNS SPF pro vaši doménu u veřejně dostupné kontroly záznamů SPF nebo DNS na webu.</span><span class="sxs-lookup"><span data-stu-id="89217-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="89217-104">Ověřte, že odchozí zpráva nebyla společností Microsoft identifikována jako spam a směrována prostřednictvím fondu pro doručování s vysokým [rizikem.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="89217-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="89217-105">Zprávy ve fondu pro doručování s vysokým rizikem neprojdou kontrolami SPF, a proto nebudou akceptovány cílovou e-mailovou organizací.</span><span class="sxs-lookup"><span data-stu-id="89217-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="89217-106">Pokud problém potrvá, budete možná muset kontaktovat správce hostitele pošty, kterému se pokoušíte poslat e-mail.</span><span class="sxs-lookup"><span data-stu-id="89217-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="89217-107">Poznamenejte si podrobnou externí chybu dostupnou ve zprávě o opuštění.</span><span class="sxs-lookup"><span data-stu-id="89217-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="89217-108">Podpora Microsoftu nemusí být schopná dále pomáhat.</span><span class="sxs-lookup"><span data-stu-id="89217-108">Microsoft support may not be able to assist further.</span></span>
