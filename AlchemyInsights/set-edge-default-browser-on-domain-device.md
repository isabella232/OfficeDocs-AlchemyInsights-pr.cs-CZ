---
title: Nastavení Microsoft Edge jako výchozího prohlížeče na zařízení připojeném k doméně
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491370"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="0a25e-102">Nastavení Microsoft Edge jako výchozího prohlížeče na zařízení připojeném k doméně</span><span class="sxs-lookup"><span data-stu-id="0a25e-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="0a25e-103">Jako výchozí prohlížeč nastavte Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="0a25e-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="0a25e-104">[Vytvořte výchozí konfigurační soubor přidružení](https://go.microsoft.com/fwlink/?linkid=2132437) a uložte ho místně nebo do sdílené síťové složky.</span><span class="sxs-lookup"><span data-stu-id="0a25e-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="0a25e-105">Otevřete editor Zásady skupiny a pak přejděte na **Šablony** pro správu konfigurace počítače  >    >  **Průzkumník souborů součástí systému Windows**  >  .</span><span class="sxs-lookup"><span data-stu-id="0a25e-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="0a25e-106">Vyberte **Nastavit výchozí konfigurační soubor přidružení**.</span><span class="sxs-lookup"><span data-stu-id="0a25e-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="0a25e-107">Vyberte **Nastavení zásad** a pak vyberte **Povoleno**.</span><span class="sxs-lookup"><span data-stu-id="0a25e-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="0a25e-108">V **části** Možnosti zadejte umístění výchozího konfiguračního souboru přidružení a pak vyberte **OK.**</span><span class="sxs-lookup"><span data-stu-id="0a25e-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
