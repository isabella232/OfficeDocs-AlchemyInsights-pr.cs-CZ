---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821440"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ca7b6-102">Řešení problémů s doručováním kódu chyby 550 5.4.1 Přístup k přenosu byl odepřen</span><span class="sxs-lookup"><span data-stu-id="ca7b6-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ca7b6-103">K tomuto problému dochází [při kontrole,](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) jestli je platná e-mailová adresa, aby se při zadávání do sítě Microsoft zabránilo návratu zpět.</span><span class="sxs-lookup"><span data-stu-id="ca7b6-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="ca7b6-104">Vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="ca7b6-104">Try the following:</span></span>

1. <span data-ttu-id="ca7b6-105">Zjistěte, jestli je problém specifický pro celou doménu nebo jednu e-mailovou adresu:</span><span class="sxs-lookup"><span data-stu-id="ca7b6-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ca7b6-106">Celá doména: Někdy je potřeba doménu synchronizovat. zkuste [nastavit doménu na Interní a potom zpátky na Autoritativní](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="ca7b6-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ca7b6-107">Jedna e-mailová adresa: Někdy je potřeba adresu synchronizovat. může pomoct změna adresy proxy serveru smtp a jeho zpětná změna.</span><span class="sxs-lookup"><span data-stu-id="ca7b6-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ca7b6-108">Zjistěte, jestli je problém specifický pro skupinu nebo veřejnou složku.</span><span class="sxs-lookup"><span data-stu-id="ca7b6-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ca7b6-109">U některých typů objektů může být potřeba objekty vytvořit ručně ve službě Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ca7b6-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ca7b6-110">Pokud potřebujete další pomoc, otevřete lístek podpory a zadejte rozsah problému (včetně typu objektu, na který odesíláte), abychom vám mohli pomoct lépe.</span><span class="sxs-lookup"><span data-stu-id="ca7b6-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>