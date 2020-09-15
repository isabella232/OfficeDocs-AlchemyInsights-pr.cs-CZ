---
title: Práce s aplikacemi VPP v systému iOS – ID pravidla 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688939"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="8da73-102">Práce s aplikacemi VPP v iOS</span><span class="sxs-lookup"><span data-stu-id="8da73-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="8da73-103">Přečtěte si, [jak spravovat aplikace pro iOS zakoupené prostřednictvím programu Volume-purchase s Microsoft Intune s](https://docs.microsoft.com/intune/vpp-apps-ios) informacemi o funkcích, omezeních a krocích, jak používat program Apple Volume purchase a podporu pro něj v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8da73-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="8da73-104">**Běžné problémy:** "Přidělil (a) aplikaci VPP aplikace Skype, ale instalace se nezdařila."</span><span class="sxs-lookup"><span data-stu-id="8da73-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="8da73-105">K tomu může dojít, pokud je jeden token VPP použit napříč více poskytovateli správy mobilních zařízení.</span><span class="sxs-lookup"><span data-stu-id="8da73-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="8da73-106">Tokeny VPP z Apple se můžou používat jenom s jedním poskytovatelem.</span><span class="sxs-lookup"><span data-stu-id="8da73-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="8da73-107">Pokud jste použili token VPP s víc poskytovateli, musíte ho znovu nahrát do Intune.</span><span class="sxs-lookup"><span data-stu-id="8da73-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="8da73-108">Instalace se může zdařit také v případě, že celkový počet instalací přesáhne počet licencí.</span><span class="sxs-lookup"><span data-stu-id="8da73-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="8da73-109">Pokud chcete zobrazit sestavu využití licencí, přejděte na stránku aplikace **Intune Mobile Apps** – \> **licence** .</span><span class="sxs-lookup"><span data-stu-id="8da73-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="8da73-110">Informace o tom, jak si vyžádat licence používané, najdete v [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="8da73-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
