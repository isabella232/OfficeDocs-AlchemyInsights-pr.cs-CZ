---
title: Problémy s instalací programu Microsoft Defender na Mac nebo Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713388"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="b43e9-102">Problémy s instalací programu Microsoft Defender na Mac nebo Linux</span><span class="sxs-lookup"><span data-stu-id="b43e9-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="b43e9-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="b43e9-103">**Mac**</span></span>

- <span data-ttu-id="b43e9-104">Před instalací atp pro Mac v programu Microsoft Defender se ujistěte, že jsou splněné požadavky na systém.</span><span class="sxs-lookup"><span data-stu-id="b43e9-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="b43e9-105">Další informace najdete v článku o instalaci programu [Microsoft Defender ATP pro Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="b43e9-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="b43e9-106">Zkontrolujte informace v souboru: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="b43e9-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="b43e9-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="b43e9-107">**Linux**</span></span>

- <span data-ttu-id="b43e9-108">Před instalací programu Microsoft Defender ATP pro Linux ověřte, že jsou splněné požadavky na systém.</span><span class="sxs-lookup"><span data-stu-id="b43e9-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="b43e9-109">Další informace najdete v článku o instalaci programu [Microsoft Defender ATP pro Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="b43e9-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="b43e9-110">Pokud chcete ověřit, jestli je služba MDATP spuštěná, podívejte se, [jestli se instalace nezdařila.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="b43e9-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="b43e9-111">Pokud chcete vyřešit a vyřešit problémy, pokud služba není spuštěná, podívejte se na postup řešení, pokud služba [mdatp není spuštěná.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="b43e9-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="b43e9-112">Postup pro kontrolu konfigurace klienta, který ověří stav produktu, a spuštění testovacího zjišťování u textového souboru EICAR, najdete v [části Konfigurace klienta.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="b43e9-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="b43e9-113">**Poznámka** Seznam podporovaných souborových systémů pro aktivitu při přístupu najdete v programu [Microsoft Defender ATP pro Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="b43e9-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>