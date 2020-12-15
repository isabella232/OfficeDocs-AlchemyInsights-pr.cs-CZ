---
title: 'Poradce při potížích s hlasem '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677018"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="0b07e-102">Poradce při potížích s hlasem</span><span class="sxs-lookup"><span data-stu-id="0b07e-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="0b07e-103">Ujistěte se, že je zaneprázdněná funkce Busy.</span><span class="sxs-lookup"><span data-stu-id="0b07e-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="0b07e-104">Pokud tento uživatel nepotřebuje tuto funkci, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="0b07e-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="0b07e-105">Přejděte do [centra pro správu týmů](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="0b07e-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="0b07e-106">Na levé straně: zásady **hlasového**  >  **volání** navigace  >   v zásadách **volání**</span><span class="sxs-lookup"><span data-stu-id="0b07e-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="0b07e-107">Vyberte **Spravovat uživatele**.</span><span class="sxs-lookup"><span data-stu-id="0b07e-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="0b07e-108">Vyhledávání uživatele a změna způsobu volání, který je zaneprázdněný, **je k dispozici, když je hovor** **vypnutý**.</span><span class="sxs-lookup"><span data-stu-id="0b07e-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="0b07e-109">Klikněte na **Použít**.</span><span class="sxs-lookup"><span data-stu-id="0b07e-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="0b07e-110">Replikace změn zásad může trvat až 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="0b07e-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="0b07e-111">Další informace o této funkci najdete v článku o tom, jak [používat: zaneprázdněn je při volání dostupný](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="0b07e-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
