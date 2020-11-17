---
title: Použití nástroje pro nasazení Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085825"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="dd815-102">Použití nástroje pro nasazení Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="dd815-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="dd815-103">K nasazení Office 365 verze Office se používá nástroj pro nasazení Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="dd815-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="dd815-104">Nástroj pro nasazení Office (setupodt.exe) se spouští z příkazového řádku a pomocí konfiguračního souboru XML zjistíte, jaké nastavení se použije při nasazení Office.</span><span class="sxs-lookup"><span data-stu-id="dd815-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="dd815-105">Stáhněte si nejnovější verzi nástroje pro nasazení Office z [webu Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="dd815-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="dd815-106">Pomocí [Nástroje pro přizpůsobení Office (OCT)](https://config.office.com) vyberte Předvolby nasazení a vytvořte konfigurační soubor XML.</span><span class="sxs-lookup"><span data-stu-id="dd815-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="dd815-107">Exportujte konfigurační soubor a umístěte ho místně do stejné složky, kde se setupodt.exe nachází.</span><span class="sxs-lookup"><span data-stu-id="dd815-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="dd815-108">**Poznámka:** Problémy s instalací Office se obvykle vyskytují v důsledku chybně nakonfigurovaných nebo malformatted konfiguračních souborů.</span><span class="sxs-lookup"><span data-stu-id="dd815-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="dd815-109">Abyste předešli těmto problémům, doporučujeme vytvořit konfigurační soubor pomocí nástroje pro přizpůsobení Office.</span><span class="sxs-lookup"><span data-stu-id="dd815-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="dd815-110">Můžete taky importovat stávající konfigurační soubory do nástroje pro přizpůsobení Office.</span><span class="sxs-lookup"><span data-stu-id="dd815-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="dd815-111">Na příkazovém řádku se zvýšenými oprávněními přejděte do umístění, kde se setupodt.exe nachází, a spusťte nástroj pro nasazení Office v režimu stahování a zadejte konfigurační soubor, který jste právě uložili.</span><span class="sxs-lookup"><span data-stu-id="dd815-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="dd815-112">V tomto příkladu je konfigurační soubor pojmenovaný Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="dd815-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="dd815-113">4. Spusťte nástroj pro nasazení Office v režimu konfigurace a určete konfigurační soubor.</span><span class="sxs-lookup"><span data-stu-id="dd815-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="dd815-114">**Poznámka:** Tento krok musíte spustit z klientského počítače, na který chcete nainstalovat Office, a musíte mít na tomto počítači oprávnění místního správce.</span><span class="sxs-lookup"><span data-stu-id="dd815-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="dd815-115">Další informace o používání nástroje pro nasazení Office pro aplikace Microsoft 365 pro podnikové scénáře nasazení pro podniky najdete v tématu [Přehled nástroje pro nasazení Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="dd815-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="dd815-116">Další podrobnosti o používání nástroje pro přizpůsobení Office najdete v tématu [Přehled nástroje pro přizpůsobení Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="dd815-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
