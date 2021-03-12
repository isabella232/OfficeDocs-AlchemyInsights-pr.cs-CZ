---
title: Řešení běžných problémů s formátováním záznamů DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744885"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="eb746-102">Řešení běžných problémů s formátováním záznamů DKIM</span><span class="sxs-lookup"><span data-stu-id="eb746-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="eb746-103">Většina problémů s nastavením DKIM souvisí s nesprávnými záznamy DNS.</span><span class="sxs-lookup"><span data-stu-id="eb746-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="eb746-104">Pokud chcete vyřešit problémy s nastavením DKIM, ověřte, jestli je záznam DKIM CNAME **(ne** záznam TXT) správně naformátovaný.</span><span class="sxs-lookup"><span data-stu-id="eb746-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="eb746-105">Další informace najdete v článku Co je potřeba udělat pro ruční nastavení [DKIM v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)</span><span class="sxs-lookup"><span data-stu-id="eb746-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="eb746-106">Pokud potřebujete obecně pomoct se záznamy DNS, podívejte se na stránku Vytvoření záznamů DNS u libovolného poskytovatele hostingu [DNS pro Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="eb746-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="eb746-107">Po vytvoření nebo aktualizaci záznamů DNS DKIM v hostitelské službě DNS pro vaši doménu budete muset počkat, až se záznamy DNS rozšíří.</span><span class="sxs-lookup"><span data-stu-id="eb746-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
