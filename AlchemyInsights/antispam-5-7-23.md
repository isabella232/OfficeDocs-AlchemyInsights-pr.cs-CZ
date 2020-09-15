---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717318"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="fbf65-102">Řešení problémů s doručováním e-mailů pro kód chyby 5.7.23</span><span class="sxs-lookup"><span data-stu-id="fbf65-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="fbf65-103">Ověřte záznam služby SPF DNS pro vaši doménu u veřejně dostupné kontroly záznamů SPF nebo DNS na webu.</span><span class="sxs-lookup"><span data-stu-id="fbf65-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="fbf65-104">Ověřte, že odchozí zpráva nebyla označena jako spam Microsoftu a směrována přes [vysoce rizikový fond](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="fbf65-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="fbf65-105">Zprávy ve vysokém fondu pro doručování rizika neprojde kontroly SPF, a proto je cílová e-mailová organizace nepřijme.</span><span class="sxs-lookup"><span data-stu-id="fbf65-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="fbf65-106">Pokud potíže potrvají, obraťte se na správce hostitele pošty, na který se pokoušíte odeslat e-mail.</span><span class="sxs-lookup"><span data-stu-id="fbf65-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="fbf65-107">Poznamenejte si podrobnou externí chybu, která je k dispozici ve zprávě o vrácení.</span><span class="sxs-lookup"><span data-stu-id="fbf65-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="fbf65-108">Podporu Microsoftu nepůjde dále podporovat.</span><span class="sxs-lookup"><span data-stu-id="fbf65-108">Microsoft support may not be able to assist further.</span></span>
