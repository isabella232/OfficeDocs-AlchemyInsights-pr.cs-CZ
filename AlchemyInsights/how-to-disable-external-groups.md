---
title: Jak zakázat externí skupiny
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704121"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="f806f-102">Jak zakázat externí skupiny</span><span class="sxs-lookup"><span data-stu-id="f806f-102">How to disable External Groups</span></span>

<span data-ttu-id="f806f-103">Externí zasílání zpráv Yammeru používá pravidla přenosu Exchange (vynucovat), což je sada proaktivních ovládacích prvků, které brání sdílení informací o společnosti.</span><span class="sxs-lookup"><span data-stu-id="f806f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="f806f-104">Aby uživatelé mohli vytvářet externí skupiny, musíte nakonfigurovat pravidlo přenosu Exchange (ETR) a potom Yammer nakonfigurovat tak, aby používal pravidlo přenosu Exchange pro blokování externích zpráv.</span><span class="sxs-lookup"><span data-stu-id="f806f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="f806f-105">Po vytvoření pravidla v centru pro správu Exchange Online nastavte ETR na použít v Yammeru takto:</span><span class="sxs-lookup"><span data-stu-id="f806f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="f806f-106">Přihlaste se k Yammeru jako ověřený správce a v **centru pro správu Yammeru**přejděte na obsah C **a \> nastavení zabezpečení.**</span><span class="sxs-lookup"><span data-stu-id="f806f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="f806f-107">V části **externí zasílání zpráv**vyberte **v Yammeru vynutit pravidla přenosu Exchange Online (vynucovat).**</span><span class="sxs-lookup"><span data-stu-id="f806f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="f806f-108">Zvolte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="f806f-108">Choose **Save**.</span></span>

<span data-ttu-id="f806f-109">Další informace najdete v článku [zakázání externího zasílání zpráv v síti Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="f806f-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  