---
title: Konfigurace vyloučení pro Microsoft Defender ATP kontroly
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
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543678"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="7dca8-102">Konfigurace vyloučení pro Microsoft Defender ATP kontroly</span><span class="sxs-lookup"><span data-stu-id="7dca8-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="7dca8-103">Obecně platí, že některé přípony souborů a umístění složek můžete z Microsoft Defender ATP souborů.</span><span class="sxs-lookup"><span data-stu-id="7dca8-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="7dca8-104">Můžete taky nakonfigurovat vyloučení souborů otevřených určitými procesy.</span><span class="sxs-lookup"><span data-stu-id="7dca8-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="7dca8-105">Další informace najdete v [tématu](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) Konfigurace a ověření vyloučení na základě přípony souboru a umístění složky a Konfigurace vyloučení souborů [otevřených procesy](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="7dca8-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="7dca8-106">Informace o konfiguraci vyloučení pro **Windows Server 2016 a 2019** najdete v tématu Konfigurace Antivirová ochrana v programu Microsoft Defender vyloučení na [Windows Serveru](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="7dca8-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="7dca8-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="7dca8-107">**Mac**</span></span>

<span data-ttu-id="7dca8-108">Podrobnosti o podporovaných typech vyloučení a konfiguraci seznamu [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) vyloučení pro Mac najdete v tématu Podporované typy vyloučení a Postup konfigurace seznamu [výjimek](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="7dca8-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="7dca8-109">**Poznámka:** Seznamy vyloučení můžete také ověřit pomocí testovacího souboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="7dca8-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="7dca8-110">Další informace najdete v tématu [Ověření seznamů vyloučení pomocí testovacího souboru EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="7dca8-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="7dca8-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="7dca8-111">**Linux**</span></span>

<span data-ttu-id="7dca8-112">Podrobnosti o podporovaných typech vyloučení a konfiguraci seznamu [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) vyloučení pro Linux najdete v tématu Podporované typy vyloučení a Konfigurace a ověření vyloučení pro Microsoft Defender ATP [pro Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="7dca8-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="7dca8-113">**Poznámka:** Seznamy vyloučení můžete také ověřit pomocí testovacího souboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="7dca8-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="7dca8-114">Další informace najdete v tématu [Ověření seznamů vyloučení pomocí testovacího souboru EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="7dca8-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 