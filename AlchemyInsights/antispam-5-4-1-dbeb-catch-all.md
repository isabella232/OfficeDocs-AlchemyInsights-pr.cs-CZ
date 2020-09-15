---
title: AntiSpam 5.4.1 DBEB catch – vše
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717354"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="9716f-102">Řešení problémů s doručováním kódu chyby 550 5.4.1 odepření přístupu</span><span class="sxs-lookup"><span data-stu-id="9716f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="9716f-103">K tomuto problému dochází, když se [zkontroluje, jestli e-mailová adresa není platná pro zabránění bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) při vstupu do sítě Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="9716f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="9716f-104">Vyzkoušejte toto:</span><span class="sxs-lookup"><span data-stu-id="9716f-104">Try the following:</span></span>

1. <span data-ttu-id="9716f-105">Zjistěte, jestli je problém specifický pro celou doménu nebo jednu e-mailovou adresu:</span><span class="sxs-lookup"><span data-stu-id="9716f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="9716f-106">Celá doména: doménu je někdy třeba synchronizovat. Zkuste [doménu nastavit jako interní a potom zpět na autoritativní](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="9716f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="9716f-107">Jediná e-mailová adresa: někdy je třeba adresu synchronizovat. můžete změnit adresu proxy serveru SMTP a pak ji znovu změnit.</span><span class="sxs-lookup"><span data-stu-id="9716f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="9716f-108">Zjistěte, jestli je problém specifický pro skupinu nebo veřejnou složku.</span><span class="sxs-lookup"><span data-stu-id="9716f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="9716f-109">U některých typů objektů je nutné, aby byly objekty ručně vytvořeny v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9716f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="9716f-110">Pokud potřebujete další pomoc, otevřete lístek podpory a zadejte obor problému (včetně typu objektu, na který posíláte), abychom vám mohli pomoct lépe.</span><span class="sxs-lookup"><span data-stu-id="9716f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>