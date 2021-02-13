---
title: Nasazení Microsoft Edge v iOSu, iPadU a Androidu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194462"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="f58cf-102">Nasazení Microsoft Edge v iOSu, iPadU a Androidu</span><span class="sxs-lookup"><span data-stu-id="f58cf-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="f58cf-103">Níže uvedený průvodce vám pomůže přiřadit Microsoft Edge uživatelům zařízení s iOS, iPadOS a Androidem.</span><span class="sxs-lookup"><span data-stu-id="f58cf-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="f58cf-104">Pokud jste uživatelům zablokovali registraci mobilních zařízení, nebude tento postup s průvodcem fungovat a uživatelé si budou muset nainstalovat Microsoft Edge sami.</span><span class="sxs-lookup"><span data-stu-id="f58cf-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="f58cf-105">V průvodci je popsaný tento postup:</span><span class="sxs-lookup"><span data-stu-id="f58cf-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="f58cf-106">Požadavky</span><span class="sxs-lookup"><span data-stu-id="f58cf-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="f58cf-107">Úvod</span><span class="sxs-lookup"><span data-stu-id="f58cf-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="f58cf-108">Základy</span><span class="sxs-lookup"><span data-stu-id="f58cf-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="f58cf-109">Konfigurace</span><span class="sxs-lookup"><span data-stu-id="f58cf-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="f58cf-110">Zadání</span><span class="sxs-lookup"><span data-stu-id="f58cf-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="f58cf-111">Revize a tvorba</span><span class="sxs-lookup"><span data-stu-id="f58cf-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="f58cf-112">Po dokončení kroků v průvodci budou zásady Microsoft Intune povolovat následující funkce aplikace Microsoft Edge pro firmy:</span><span class="sxs-lookup"><span data-stu-id="f58cf-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="f58cf-113">Duální identita</span><span class="sxs-lookup"><span data-stu-id="f58cf-113">Dual identity</span></span>
- <span data-ttu-id="f58cf-114">Integrace se zásadou ochrany aplikací Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f58cf-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="f58cf-115">Integrace s proxy serverem aplikace Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f58cf-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="f58cf-116">Spravované oblíbené položky a klávesové zkratky domovské stránky</span><span class="sxs-lookup"><span data-stu-id="f58cf-116">Managed favorites and home page shortcuts</span></span>
