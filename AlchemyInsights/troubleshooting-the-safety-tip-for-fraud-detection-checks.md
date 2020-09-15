---
title: Řešení potíží s bezpečnostním tipem pro kontroly rozpoznávání podvodů
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658403"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ff890-102">Řešení potíží s bezpečnostním tipem pro kontroly rozpoznávání podvodů</span><span class="sxs-lookup"><span data-stu-id="ff890-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ff890-103">Pokud se vám zobrazuje bezpečnostní tip, který říká "odesílatel selhal při kontrole vyhledávání podvodů a nepovažuje se, kdo se jeví jako", odesílatel se nepovedlo projít kontrolou ověřování DKIM nebo SPF.</span><span class="sxs-lookup"><span data-stu-id="ff890-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ff890-104">Nejlepším způsobem, jak tento problém vyřešit, je to, aby ho odesílatel sám povolil.</span><span class="sxs-lookup"><span data-stu-id="ff890-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ff890-105">Pokud odesílatel posílá vaše zastoupení, musíte ho schválit přidáním IP adresy odesílatele k záznamu SPF.</span><span class="sxs-lookup"><span data-stu-id="ff890-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ff890-106">Další informace najdete v článku [Poradce při potížích s červeným (podezřelým) bezpečnostním tipem pro detekci podvodů](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="ff890-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="ff890-107">Tady je několik dalších odkazů, které vám můžou pomoct:</span><span class="sxs-lookup"><span data-stu-id="ff890-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ff890-108">Jak Microsoft používá k zabránění falšování identity architekturu zásad pro odesílatele (SPF)</span><span class="sxs-lookup"><span data-stu-id="ff890-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="ff890-109">Nastavení SPF pro zabránění falšování obsahu</span><span class="sxs-lookup"><span data-stu-id="ff890-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
