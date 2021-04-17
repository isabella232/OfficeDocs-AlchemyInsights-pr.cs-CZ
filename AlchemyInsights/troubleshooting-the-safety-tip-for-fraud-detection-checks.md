---
title: Řešení potíží s bezpečnostním tipem pro kontroly zjišťování podvodů
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834724"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="2ee09-102">Řešení potíží s bezpečnostním tipem pro kontroly zjišťování podvodů</span><span class="sxs-lookup"><span data-stu-id="2ee09-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="2ee09-103">Pokud se vám zobrazí bezpečnostní tip s informací, že odesílatel neprošel našimi kontrolami zjišťování podvodů a nemusí být tím, kým se jeví, pak odesílatel neprošel kontrolami ověřování DKIM nebo SPF.</span><span class="sxs-lookup"><span data-stu-id="2ee09-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="2ee09-104">Nejlepší způsob, jak to vyřešit, je, aby odesílatel autorizuje sám sebe.</span><span class="sxs-lookup"><span data-stu-id="2ee09-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="2ee09-105">Pokud odesílatel posílá vaším jménem, musíte ho autorizovat přidáním IP adresy odesílatele do záznamu SPF.</span><span class="sxs-lookup"><span data-stu-id="2ee09-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="2ee09-106">Další informace najdete v článku Řešení potíží s [červeným (podezřelým)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) bezpečnostním tipem pro zjišťování podvodů.</span><span class="sxs-lookup"><span data-stu-id="2ee09-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="2ee09-107">Tady jsou některé další odkazy, které vám pomůžou:</span><span class="sxs-lookup"><span data-stu-id="2ee09-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="2ee09-108">Jak Microsoft používá rozhraní SPF (Sender Policy Framework) k zabránění falšování falšování</span><span class="sxs-lookup"><span data-stu-id="2ee09-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="2ee09-109">Nastavení SPF, aby se zabránilo falšování falšování</span><span class="sxs-lookup"><span data-stu-id="2ee09-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
