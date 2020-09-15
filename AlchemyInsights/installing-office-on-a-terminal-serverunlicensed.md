---
title: Instalace Office na terminálový server – nelicencovaná
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663110"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8f67c-102">Instalace Office na terminálový server</span><span class="sxs-lookup"><span data-stu-id="8f67c-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8f67c-103">Pro nasazení aplikací Microsoft 365 pro podnik na Windows serveru pomocí vzdálené plochy (RDS), dřív s názvem Terminálová služba:</span><span class="sxs-lookup"><span data-stu-id="8f67c-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8f67c-104">Musíte mít předplatné Microsoft 365, které obsahuje aplikace Microsoft 365 pro podniky, jako je třeba Office 365 Enterprise E3 nebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8f67c-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8f67c-105">Plány aplikací Microsoft 365 pro firmy a Microsoft 365 Apps for Business Premium neobsahují aplikace Microsoft 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="8f67c-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="8f67c-106">Je třeba povolit [aktivaci sdílené počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8f67c-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="8f67c-107">Pokud chcete nainstalovat aplikace Microsoft 365 pro podnik v rámci služby RDS z centra pro správu Microsoft 365, ***které používá výchozí nastavení instalace***, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="8f67c-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8f67c-108">Můžete také stáhnout a spustit [Pomocníka pro podporu a obnovení Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pro systém Microsoft 365 v režimu aktivace sdíleného počítače.</span><span class="sxs-lookup"><span data-stu-id="8f67c-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8f67c-109">Podívejte se na předplatné Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8f67c-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="8f67c-110">Zjistěte, jak</span><span class="sxs-lookup"><span data-stu-id="8f67c-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8f67c-111">V případě potřeby přejděte na jiné předplatné Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8f67c-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="8f67c-112">Zjistěte, jak</span><span class="sxs-lookup"><span data-stu-id="8f67c-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="8f67c-113">Pokud už máte Office nainstalovaný na serveru RDS pomocí jakéhokoli jiného předplatného Microsoft 365, odinstalujte ho.</span><span class="sxs-lookup"><span data-stu-id="8f67c-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="8f67c-114">Například v ovládacím panelu \> Odinstalujte program.</span><span class="sxs-lookup"><span data-stu-id="8f67c-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8f67c-115">Pokud máte problémy, odinstalujte ho pomocí nástroje [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="8f67c-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8f67c-116">Na serveru RDS se přihlaste do centra pro správu Microsoft 365 s účtem správce a [nainstalujte si aplikace Microsoft 365 pro podniky](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8f67c-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8f67c-117">Po instalaci Office se ***Neotevírejte ani se přihlaste*** k žádným aplikacím Office.</span><span class="sxs-lookup"><span data-stu-id="8f67c-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8f67c-118">Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru pomocí následujícího postupu:</span><span class="sxs-lookup"><span data-stu-id="8f67c-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8f67c-119">Klikněte pravým tlačítkem myši na tlačítko Windows v levém dolním rohu obrazovky a vyberte spustit.</span><span class="sxs-lookup"><span data-stu-id="8f67c-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8f67c-120">Do pole Otevřít zadejte **Regedit**a pak vyberte OK.</span><span class="sxs-lookup"><span data-stu-id="8f67c-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8f67c-121">Když se zobrazí výzva, aby Editor registru mohl v zařízení dělat změny, vyberte Ano.</span><span class="sxs-lookup"><span data-stu-id="8f67c-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8f67c-122">V editoru registru přidejte hodnotu řetězce **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8f67c-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8f67c-123">Na serveru RDS se ***přihlaste jako koncový uživatel*** a [Ověřte, jestli je povolená aktivace sdíleného počítače pro Microsoft 365](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8f67c-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="8f67c-124">Další informace o požadavcích, pokyny k instalaci a pokyny k přizpůsobení instalací pomocí nástroje pro nasazení Office najdete v článku [nasazení aplikací Microsoft 365 pro podnik pomocí služby Vzdálená plocha](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8f67c-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="8f67c-125">Pokud chcete opravit chyby související s aktivací sdíleného počítače, přečtěte si článek [Poradce při potížích s aktivací sdílené počítače pro aplikace Microsoft 365 pro podnik](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8f67c-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  