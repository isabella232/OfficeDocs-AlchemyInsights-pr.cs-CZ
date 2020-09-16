---
title: Řešení problémů s ověřováním SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737982"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="c710d-102">Řešení problémů s ověřováním SMTP</span><span class="sxs-lookup"><span data-stu-id="c710d-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="c710d-103">Pokud se při pokusu o odeslání e-mailu SMTP a ověřování pomocí klienta nebo aplikace dostanou chyby 5.7.57 nebo 5.7.3, je potřeba zkontrolovat:</span><span class="sxs-lookup"><span data-stu-id="c710d-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="c710d-104">Ověřené odeslání protokolu SMTP může být zakázáno ve vašem tenantovi nebo v poštovní schránce, kterou chcete použít (zaškrtněte obě políčka).</span><span class="sxs-lookup"><span data-stu-id="c710d-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="c710d-105">Další informace najdete v článku [Povolení nebo zákaz odesílání ověřených klientů SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="c710d-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="c710d-106">Zkontrolujte, jestli jsou pro tenanta povolené [výchozí hodnoty zabezpečení Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) . Pokud je tato možnost povolená, ověřování SMTP pomocí základního ověřování (známé také jako starší verze) se nezdaří.</span><span class="sxs-lookup"><span data-stu-id="c710d-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
