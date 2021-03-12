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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744530"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="04160-102">Povolení vlastní domény pro DKIM</span><span class="sxs-lookup"><span data-stu-id="04160-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="04160-103">Po vytvoření záznamů CNAME pro vlastní domény je potřeba doménu povolit.</span><span class="sxs-lookup"><span data-stu-id="04160-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="04160-104">Pokud chcete doménu povolit, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="04160-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="04160-105">Přejděte do [Centra pro správu Exchange](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="04160-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="04160-106">V levém podokně vyberte ochrana **> dkim**.</span><span class="sxs-lookup"><span data-stu-id="04160-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="04160-107">Vyberte doménu a v části Podepisovat zprávy pro tuto doménu **pomocí podpisů DKIM** klikněte na **Povolit.**</span><span class="sxs-lookup"><span data-stu-id="04160-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="04160-108">Tento krok opakujte pro každou doménu.</span><span class="sxs-lookup"><span data-stu-id="04160-108">Repeat this step for each domain.</span></span>

