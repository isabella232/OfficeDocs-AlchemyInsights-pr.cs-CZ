---
title: Konfigurace vyloučení pro kontrolu atp v programu Microsoft Defender
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713400"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="50605-102">Konfigurace vyloučení pro kontrolu atp v programu Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="50605-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="50605-103">Obecně platí, že určité přípony souborů a umístění složek můžete z naskenování atp v programu Microsoft Defender vyloučit.</span><span class="sxs-lookup"><span data-stu-id="50605-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="50605-104">Můžete taky nakonfigurovat vyloučení u souborů otevřených určitými procesy.</span><span class="sxs-lookup"><span data-stu-id="50605-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="50605-105">Další informace najdete v tématu Konfigurace a [ověření](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) vyloučení na základě přípony souboru a umístění složky a Konfigurace vyloučení u souborů [otevřených procesy.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="50605-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="50605-106">Pokud chcete nakonfigurovat vyloučení pro **Windows Server 2016 a 2019,** podívejte se na článek Konfigurace vyloučení antivirové ochrany v programu [Microsoft Defender na Windows Serveru.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="50605-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="50605-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="50605-107">**Mac**</span></span>

<span data-ttu-id="50605-108">Podrobnosti o podporovaných typech vyloučení a konfiguraci seznamu [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) vyloučení pro Mac najdete v tématu Podporované typy vyloučení a Jak nakonfigurovat seznam [vyloučení.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="50605-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="50605-109">**Poznámka** Seznamy vyloučení můžete také ověřit pomocí testovacího souboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="50605-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="50605-110">Další informace najdete v článku [o ověření seznamů vyloučení pomocí testovacího souboru EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="50605-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="50605-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="50605-111">**Linux**</span></span>

<span data-ttu-id="50605-112">Podrobnosti o podporovaných typech vyloučených položek a [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) konfiguraci seznamu vyloučení v Linuxu najdete v tématu Podporované typy vyloučení a Konfigurace a ověření vyloučení z programu [Microsoft Defender ATP pro Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="50605-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="50605-113">**Poznámka** Seznamy vyloučení můžete také ověřit pomocí testovacího souboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="50605-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="50605-114">Další informace najdete v článku [o ověření seznamů vyloučení pomocí testovacího souboru EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="50605-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 