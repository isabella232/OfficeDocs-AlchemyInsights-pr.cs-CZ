---
title: Povolení vlastní domény pro DKIM
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
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523612"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="f10aa-102">Povolení vlastní domény pro DKIM</span><span class="sxs-lookup"><span data-stu-id="f10aa-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="f10aa-103">Po vytvoření záznamů CNAME pro vlastní domény je potřeba tuto doménu povolit.</span><span class="sxs-lookup"><span data-stu-id="f10aa-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="f10aa-104">Pokud chcete doménu povolit, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="f10aa-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="f10aa-105">Přejděte do [Centra pro správu Exchange.](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="f10aa-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="f10aa-106">V levém podokně vyberte ochranu > **dkim.**</span><span class="sxs-lookup"><span data-stu-id="f10aa-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="f10aa-107">Vyberte doménu a potom v části Podepisovat zprávy pro tuto doménu **pomocí podpisů DKIM** klikněte na **Povolit.**</span><span class="sxs-lookup"><span data-stu-id="f10aa-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="f10aa-108">Tento krok opakujte pro každou doménu.</span><span class="sxs-lookup"><span data-stu-id="f10aa-108">Repeat this step for each domain.</span></span>

