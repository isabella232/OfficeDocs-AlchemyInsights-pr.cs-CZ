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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/10/2020
ms.locfileid: "49677102"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="4293c-102">Použití Microsoft Intune ke správě webového přístupu v Microsoft Edge pro iOS a Android</span><span class="sxs-lookup"><span data-stu-id="4293c-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="4293c-103">Microsoft Edge pro iOS a Android umožňuje uživatelům procházet web z více úplně oddělených profilů.</span><span class="sxs-lookup"><span data-stu-id="4293c-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="4293c-104">Možnosti široké ochrany dat pro Microsoft 365 jsou dostupné, když se přihlásíte k odběru Enterprise mobility a bezpečnostní sady, která zahrnuje funkce Microsoft Intune a Azure Active Directory Premium, jako je třeba podmíněný přístup.</span><span class="sxs-lookup"><span data-stu-id="4293c-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="4293c-105">Je třeba nasadit zásadu podmíněného přístupu, která (1) umožňuje uživatelům připojení z mobilních zařízení do Microsoft Edge pro iOS a Android a že (2) implementuje zásady ochrany aplikací Microsoft Intune, které poskytují chráněné možnosti procházení.</span><span class="sxs-lookup"><span data-stu-id="4293c-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="4293c-106">Informace o používání podmíněného přístupu a zásad najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="4293c-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="4293c-107">Použití zásad podmíněného přístupu služby Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4293c-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="4293c-108">Vytvoření zásad ochrany aplikací Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4293c-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="4293c-109">Použití jednotného přihlašování pro Azure Active Directory – připojené webové aplikace v prohlížečích chráněných zásadami</span><span class="sxs-lookup"><span data-stu-id="4293c-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="4293c-110">Správa možností procházení pomocí konfigurace aplikace</span><span class="sxs-lookup"><span data-stu-id="4293c-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="4293c-111">Povolit používání pouze pracovních a školních účtů</span><span class="sxs-lookup"><span data-stu-id="4293c-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="4293c-112">Nasazení obecných zásad konfigurace aplikace</span><span class="sxs-lookup"><span data-stu-id="4293c-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="4293c-113">Nasazení zásad konfigurace aplikace pro ochranu dat</span><span class="sxs-lookup"><span data-stu-id="4293c-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="4293c-114">Nasazení zásad konfigurace aplikací pomocí služby Microsoft Endpoint Manager</span><span class="sxs-lookup"><span data-stu-id="4293c-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="4293c-115">Informace o tom, jak získat přístup k protokolům spravovaných aplikací, najdete v tématu [použití Microsoft Edge pro iOS a Android pro přístup k protokolům spravovaných aplikací](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="4293c-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
