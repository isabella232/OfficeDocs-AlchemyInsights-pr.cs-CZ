---
title: Řešení problémů s ověřováním SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264365"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="6e9be-102">Řešení problémů s ověřováním SMTP</span><span class="sxs-lookup"><span data-stu-id="6e9be-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="6e9be-103">Pokud se při pokusu o odeslání e-mailu SMTP a ověření pomocí klienta nebo aplikace zobrazí chyby 5.7.57 nebo 5.7.3, měli byste zkontrolovat:</span><span class="sxs-lookup"><span data-stu-id="6e9be-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="6e9be-104">Ověřené odesílání protokolu SMTP může být zakázáno ve vašem tenantovi nebo v poštovní schránce, kterou se pokoušíte použít (zkontrolujte obě nastavení).</span><span class="sxs-lookup"><span data-stu-id="6e9be-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="6e9be-105">Další informace naleznete v tématu [Povolení nebo zakázání odeslání ověřovacího klienta SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="6e9be-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="6e9be-106">Zkontrolujte, jestli jsou pro vašeho tenanta [povolené výchozí hodnoty zabezpečení Azure.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) Pokud je povoleno, ověřování SMTP pomocí základního ověřování (označované také jako starší verze; to bude používat uživatelské jméno a heslo) se nezdaří.</span><span class="sxs-lookup"><span data-stu-id="6e9be-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
