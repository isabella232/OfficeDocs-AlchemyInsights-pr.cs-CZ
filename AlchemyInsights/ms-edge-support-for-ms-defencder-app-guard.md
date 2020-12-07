---
title: Podpora Microsoftu pro Microsoft Edge pro ochranu Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583366"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="823f4-102">Podpora Microsoftu pro Microsoft Edge pro ochranu Application Guard</span><span class="sxs-lookup"><span data-stu-id="823f4-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="823f4-103">Pro Windows 10 a Microsoft Edge používá funkce Guard přístup k izolaci hardwaru, pomocí kterého může uživatel přejít na nedůvěryhodný web z izolovaného kontejneru povoleného technologií Hyper-V, který je oddělen od hostitelského operačního systému.</span><span class="sxs-lookup"><span data-stu-id="823f4-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="823f4-104">Správce rozlehlé sítě definuje seznam důvěryhodných webů, cloudových zdrojů a interních sítí.</span><span class="sxs-lookup"><span data-stu-id="823f4-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="823f4-105">Když uživatel navštíví web, který není v seznamu, otevře Microsoft Edge Web v kontejneru.</span><span class="sxs-lookup"><span data-stu-id="823f4-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="823f4-106">To znamená, že pokud se web vypíná za nebezpečný, bude hostitelský počítač i nadále chráněn a útočník se nedostane do podnikových dat.</span><span class="sxs-lookup"><span data-stu-id="823f4-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="823f4-107">Instalace rozšíření v kontejneru je podporovaná od Microsoft Edge verze 81 a dá se ovládat prostřednictvím zásad.</span><span class="sxs-lookup"><span data-stu-id="823f4-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="823f4-108">Adresa updateURL, která se používá v zásadách ExtensionInstallForcelist, by se měla přidat jako neutrální prostředek do zásad izolace sítě používaných ochranou Application Guard.</span><span class="sxs-lookup"><span data-stu-id="823f4-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="823f4-109">Další informace najdete v článku [Podpora Microsoft Edge pro ochranu Application Guard pro Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="823f4-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
