---
title: Blokování podpisů e-mailů od uživatelů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243317"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="db35e-102">Blokování podpisů e-mailů od uživatelů</span><span class="sxs-lookup"><span data-stu-id="db35e-102">Block user-made email signatures</span></span>

<span data-ttu-id="db35e-103">Následující řešení platí jenom pro podpisy e-mailů vytvořené v Outlooku na webu.</span><span class="sxs-lookup"><span data-stu-id="db35e-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="db35e-104">Podpisy můžete v aplikaci Outlook blokovat jenom v případě, že máte místní Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="db35e-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="db35e-105">V Centru pro správu zvolte **Centra pro správu**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="db35e-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="db35e-106">Klikněte **na oprávnění zásad** Outlook Web  >  **Appu.**</span><span class="sxs-lookup"><span data-stu-id="db35e-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="db35e-107">Vyberte zásadu a pak ji kliknutím na ikonu tužky upravte.</span><span class="sxs-lookup"><span data-stu-id="db35e-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="db35e-108">Funkce **pro kliknutí** Další  >  **možnosti**</span><span class="sxs-lookup"><span data-stu-id="db35e-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="db35e-109">V **části Uživatelské prostředí** zrušte zaškrtnutí políčka **Podpis** e-mailu a klikněte na **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="db35e-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="db35e-110">**Důležité:** Pokud jste před zrušením zaškrtnutí tohoto políčka přidali podpis, uživatel ho bude moct i nadále používat.</span><span class="sxs-lookup"><span data-stu-id="db35e-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="db35e-111">Požádat je o odebrání.</span><span class="sxs-lookup"><span data-stu-id="db35e-111">Ask them to remove it.</span></span>
