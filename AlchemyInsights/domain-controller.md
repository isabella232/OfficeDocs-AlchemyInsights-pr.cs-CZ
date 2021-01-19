---
title: Řadič domény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900801"
---
# <a name="domain-controller"></a><span data-ttu-id="103ac-102">Řadič domény</span><span class="sxs-lookup"><span data-stu-id="103ac-102">Domain controller</span></span>

<span data-ttu-id="103ac-103">**Nelze povolit AAD – DS nebo nasazení se nedaří.**</span><span class="sxs-lookup"><span data-stu-id="103ac-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="103ac-104">Chcete-li vyřešit problém s povolením nebo selháním služby domény Azure AD (AAD-DS), proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="103ac-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="103ac-105">Pokud používáte už existující virtuální síť, zkontrolujte NSG pravidel, která blokují porty potřebné k synchronizaci v AAD-DS na portálu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="103ac-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="103ac-106">Zkontrolujte, jestli je v tomto průvodci odstraňováním potíží v téhle chybové zprávě odpověď, která je dostupná v  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="103ac-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="103ac-107">Zkuste nasadit služby domény Azure AD v nové virtuální síti.</span><span class="sxs-lookup"><span data-stu-id="103ac-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="103ac-108">Postupujte podle pokynů Průvodce Začínáme s postupem nasazení služby AAD-DS, která je k dispozici v [kurzu vytváření služeb domény Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="103ac-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="103ac-109">Pokud máte problémy s nasazením služeb domény Azure AD, Projděte si téma [Poradce při potížích s doménami Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kde najdete běžné chyby, které vám pomůžou začít pracovat.</span><span class="sxs-lookup"><span data-stu-id="103ac-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="103ac-110">**Nejde zakázat AAD – DS.**</span><span class="sxs-lookup"><span data-stu-id="103ac-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="103ac-111">AAD – DS nelze pozastavit.</span><span class="sxs-lookup"><span data-stu-id="103ac-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="103ac-112">Pokud chcete spravovanou doménu přestat používat, musíte ji odstranit.</span><span class="sxs-lookup"><span data-stu-id="103ac-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="103ac-113">Pokud narazíte na problémy, přečtěte si běžné chybové zprávy a související kroky řešení potíží, které vám pomůžou znovu začít pracovat, podívejte se na [řešení potíží se službou Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="103ac-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
