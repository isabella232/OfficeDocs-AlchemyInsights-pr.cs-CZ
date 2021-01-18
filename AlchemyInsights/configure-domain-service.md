---
title: Konfigurace doménové služby
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884985"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="08d74-102">Nelze povolit AAD – DS nebo nasazení se nedaří.</span><span class="sxs-lookup"><span data-stu-id="08d74-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="08d74-103">Chcete-li vyřešit problém s povolením nebo selháním služby domény Azure AD (AAD-DS), proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="08d74-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="08d74-104">Pokud používáte už existující virtuální síť, zkontrolujte NSG pravidel, která blokují porty potřebné k synchronizaci v AAD-DS na portálu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="08d74-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="08d74-105">Zkontrolujte, jestli je v tomto průvodci odstraňováním potíží v téhle chybové zprávě odpověď, která je dostupná v  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="08d74-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="08d74-106">Zkuste nasadit služby domény Azure AD v nové virtuální síti.</span><span class="sxs-lookup"><span data-stu-id="08d74-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="08d74-107">Postupujte podle pokynů Průvodce Začínáme s postupem nasazení [služby DNS](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="08d74-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="08d74-108">Pokud máte problémy s nasazením služeb domény Azure AD, Projděte si téma [Poradce při potížích s doménami Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kde najdete běžné chyby, které vám pomůžou začít pracovat.</span><span class="sxs-lookup"><span data-stu-id="08d74-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="08d74-109">**Nejde zakázat AAD – DS.**</span><span class="sxs-lookup"><span data-stu-id="08d74-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="08d74-110">AAD – DS nelze pozastavit.</span><span class="sxs-lookup"><span data-stu-id="08d74-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="08d74-111">Pokud chcete spravovanou doménu přestat používat, musíte ji odstranit.</span><span class="sxs-lookup"><span data-stu-id="08d74-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="08d74-112">Pokud chcete odstranit spravovanou doménu, přečtěte si článek [odstranění služby DNS AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="08d74-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



