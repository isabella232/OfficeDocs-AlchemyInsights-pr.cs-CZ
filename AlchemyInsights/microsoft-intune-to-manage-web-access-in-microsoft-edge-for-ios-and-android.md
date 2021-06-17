---
title: Použití Microsoft Intune ke správě webového přístupu v Microsoft Edge pro iOS a Android
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
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989654"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="819da-102">Použití Microsoft Intune ke správě webového přístupu v Microsoft Edge pro iOS a Android</span><span class="sxs-lookup"><span data-stu-id="819da-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="819da-103">Microsoft Edge pro iOS a Android umožňuje uživateli procházet web z několika úplně samostatných profilů.</span><span class="sxs-lookup"><span data-stu-id="819da-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="819da-104">Nejširší možnosti ochrany dat Microsoft 365 k dispozici, když se přihlásíte k odběru sady Enterprise Mobility + Security, která zahrnuje funkce Microsoft Intune a Azure Active Directory Premium, jako je podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="819da-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="819da-105">Minimálně budete chtít nasadit zásady podmíněného přístupu, které (1) umožňují uživatelům připojovat se z mobilních zařízení k Microsoft Edge pro iOS a Android a že (2) implementuje zásadu ochrany aplikací Microsoft Intune, která poskytuje chráněné prostředí procházení.</span><span class="sxs-lookup"><span data-stu-id="819da-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="819da-106">Informace o tom, jak můžete používat podmíněný přístup a zásady, najdete v tématu:</span><span class="sxs-lookup"><span data-stu-id="819da-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="819da-107">Použití Azure Active Directory zásad podmíněného přístupu</span><span class="sxs-lookup"><span data-stu-id="819da-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="819da-108">Vytvoření Microsoft Intune ochrany aplikací</span><span class="sxs-lookup"><span data-stu-id="819da-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="819da-109">Použití jednotného přihlašování pro webové Azure Active Directory aplikace připojené k internetu v prohlížečích chráněných zásadou</span><span class="sxs-lookup"><span data-stu-id="819da-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="819da-110">Správa prostředí procházení pomocí konfigurace aplikace</span><span class="sxs-lookup"><span data-stu-id="819da-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="819da-111">Povolit použití jenom pracovních a školních účtů</span><span class="sxs-lookup"><span data-stu-id="819da-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="819da-112">Nasazení obecných zásad konfigurace aplikací</span><span class="sxs-lookup"><span data-stu-id="819da-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="819da-113">Nasazení zásad konfigurace aplikací pro ochranu dat</span><span class="sxs-lookup"><span data-stu-id="819da-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="819da-114">Použití Microsoft Endpoint Manager nasazení zásad konfigurace aplikací</span><span class="sxs-lookup"><span data-stu-id="819da-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="819da-115">Informace o tom, jak získat přístup ke spravovaným protokolům aplikací, najdete v tématu Použití [Microsoft Edge pro iOS](https://go.microsoft.com/fwlink/?linkid=2132578)a Android pro přístup ke spravovaným protokolům aplikací .</span><span class="sxs-lookup"><span data-stu-id="819da-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
