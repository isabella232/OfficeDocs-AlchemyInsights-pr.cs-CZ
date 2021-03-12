---
title: Replikační sada
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713496"
---
# <a name="replica-set"></a><span data-ttu-id="3406f-102">Replikační sada</span><span class="sxs-lookup"><span data-stu-id="3406f-102">Replica set</span></span>

<span data-ttu-id="3406f-103">AADDS se taky nazývá spravovaná doména.</span><span class="sxs-lookup"><span data-stu-id="3406f-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="3406f-104">Ve skutečnosti jde o dva řadiče domény, které provozuje a udržuje back-end.</span><span class="sxs-lookup"><span data-stu-id="3406f-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="3406f-105">Tyto dvě počítače DCs zahrnují jednu hlavní dc a jednu replikační dc.</span><span class="sxs-lookup"><span data-stu-id="3406f-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="3406f-106">Zálohy ve službě AADDS (spravovaná doména) jsou automatizovaný proces spravovaný platformou Azure.</span><span class="sxs-lookup"><span data-stu-id="3406f-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="3406f-107">V případě problému se spravovanou doménou vám může pomoct podpora Azure při obnovování ze zálohy.</span><span class="sxs-lookup"><span data-stu-id="3406f-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="3406f-108">Každou sadu replik vytvoříte ve virtuální síti.</span><span class="sxs-lookup"><span data-stu-id="3406f-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="3406f-109">Každá virtuální síť se musí vzájemně na partnerský vztah používat ke každé jiné virtuální síti, která hostuje replikační sadu spravované domény.</span><span class="sxs-lookup"><span data-stu-id="3406f-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="3406f-110">Tato konfigurace vytvoří topologii sítě, která podporuje replikaci adresářů.</span><span class="sxs-lookup"><span data-stu-id="3406f-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="3406f-111">Virtuální síť může podporovat několik sad replik za předpokladu, že je každá sada replik v jiné virtuální podsíti.</span><span class="sxs-lookup"><span data-stu-id="3406f-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="3406f-112">Další podrobnosti o sadě replik najdete v tématu Sady replik [konceptů.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="3406f-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
