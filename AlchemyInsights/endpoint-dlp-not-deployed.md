---
title: Endpoint DLP not deployed to user's device
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731321"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="2f1f4-102">Endpoint DLP not deployed to user's device</span><span class="sxs-lookup"><span data-stu-id="2f1f4-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="2f1f4-103">Pokud se na zařízení uživatele nepou3/4ít nastavení Ochrana před únikem dat koncového bodu, potvrďte, že splňujete tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="2f1f4-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="2f1f4-104">Windows 10 zařízení je nainstalovaný build x64 1809 nebo novější.</span><span class="sxs-lookup"><span data-stu-id="2f1f4-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="2f1f4-105">Klient antimalwaru verze 4.18.2009.7 nebo novější je nainstalovaný.</span><span class="sxs-lookup"><span data-stu-id="2f1f4-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="2f1f4-106">Zařízení je **jedním z** těchto:</span><span class="sxs-lookup"><span data-stu-id="2f1f4-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="2f1f4-107">Azure Active Directory (Azure AD) připojeno</span><span class="sxs-lookup"><span data-stu-id="2f1f4-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="2f1f4-108">Hybridní připojení k Azure AD</span><span class="sxs-lookup"><span data-stu-id="2f1f4-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="2f1f4-109">Zaregistrovaná AAD</span><span class="sxs-lookup"><span data-stu-id="2f1f4-109">AAD registered</span></span>

- <span data-ttu-id="2f1f4-110">Pokud chcete vynutit akce zásad, ujistěte se, Chromium na zařízení koncového bodu je nainstalovaný prohlížeč Microsoft Chromium Edge.</span><span class="sxs-lookup"><span data-stu-id="2f1f4-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="2f1f4-111">Další požadavky pro nasazení funkce DLP koncového bodu najdete v tématu Začínáme s prevencí [ztráty dat koncového bodu](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="2f1f4-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>