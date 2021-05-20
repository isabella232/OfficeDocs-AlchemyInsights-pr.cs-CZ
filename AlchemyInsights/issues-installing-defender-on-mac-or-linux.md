---
title: Problémy s instalací Microsoft Defenderu na Mac nebo Linux
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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539673"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="5d339-102">Problémy s instalací Microsoft Defenderu na Mac nebo Linux</span><span class="sxs-lookup"><span data-stu-id="5d339-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="5d339-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="5d339-103">**Mac**</span></span>

- <span data-ttu-id="5d339-104">Před instalací aplikace Microsoft Defender ATP pro Mac se ujistěte, že jsou splněny požadavky na systém.</span><span class="sxs-lookup"><span data-stu-id="5d339-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="5d339-105">Další informace najdete v [článku Jak nainstalovat Microsoft Defender ATP pro Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="5d339-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="5d339-106">Zkontrolujte informace v souboru: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="5d339-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="5d339-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="5d339-107">**Linux**</span></span>

- <span data-ttu-id="5d339-108">Před instalací systému pro Linux se ujistěte, že jsou Microsoft Defender ATP požadavky na systém.</span><span class="sxs-lookup"><span data-stu-id="5d339-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="5d339-109">Další informace najdete v [článku Jak nainstalovat MDATP pro Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="5d339-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="5d339-110">Informace o tom, MDATP služba spuštěná, najdete v [tématu Instalace se nezdařila.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="5d339-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="5d339-111">Pokud chcete vyřešit a vyřešit problémy, pokud služba není spuštěná, podívejte se na postup řešení potíží, pokud služba [mdatp není spuštěná.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="5d339-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="5d339-112">Postup kontroly konfigurace klienta, který ověřuje stav produktu, a spuštění detekčního testu v textovém souboru EICAR najdete v tématu [Konfigurace klienta](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="5d339-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="5d339-113">**Poznámka:** Seznam podporovaných souborových systémů pro aktivitu při přístupu najdete v Microsoft Defender ATP [pro Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="5d339-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>