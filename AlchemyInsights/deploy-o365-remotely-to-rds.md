---
title: Nasazení aplikací Microsoft 365 pro podnik pro sdílení pro sdílené použití na RDS, terminálovém serveru nebo VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745528"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="7e8f0-102">Nasazení aplikací Microsoft 365 pro podnik pro sdílení pro sdílené použití na RDS, terminálovém serveru nebo VDI</span><span class="sxs-lookup"><span data-stu-id="7e8f0-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="7e8f0-103">Nasazení aplikací Microsoft 365 pro podnik pomocí služby Vzdálená plocha (RDS) s názvem Terminálová služba</span><span class="sxs-lookup"><span data-stu-id="7e8f0-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="7e8f0-104">Musíte mít plán Microsoft 365 pro firmy nebo plán Office 365, který zahrnuje aplikace Microsoft 365 pro podnik, jako je Office 365 Enterprise E3 nebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="7e8f0-105">Plány aplikací Microsoft 365 pro firmy a Microsoft 365 Business Premium neobsahují aplikace Microsoft 365 pro podnik.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="7e8f0-106">Musíte povolit [aktivaci sdíleného počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="7e8f0-107">Můžete také stáhnout a spustit [Pomocníka pro podporu a obnovení Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pro systém Microsoft 365 v režimu aktivace sdíleného počítače.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="7e8f0-108">Další informace o požadavcích, pokyny k instalaci a pokyny k vlastním instalacím pomocí nástroje pro nasazení Office najdete v článku [nasazení aplikací Microsoft 365 pro podnik pomocí služby Vzdálená plocha](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="7e8f0-109">Oprava chyb souvisejících se aktivací sdíleného počítače:</span><span class="sxs-lookup"><span data-stu-id="7e8f0-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="7e8f0-110">Přečtěte si článek [Poradce při potížích s aktivací sdílené počítače pro aplikace Microsoft 365 pro podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="7e8f0-111">Přečtěte si téma zaměřené na [resetování stavu aktivace Microsoft 365 Apps pro podniky](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="7e8f0-112">Pokud chcete nainstalovat aplikace Microsoft 365 pro podnik v rámci služby RDS z centra pro správu Microsoft 365, ***které používá výchozí nastavení instalace***, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="7e8f0-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="7e8f0-113">Zkontrolujte, jaké máte předplatné.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-113">Check what subscription you have.</span></span> <span data-ttu-id="7e8f0-114">[Zjistěte, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="7e8f0-115">V případě potřeby přepněte na jiné předplatné.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="7e8f0-116">[Zjistěte, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="7e8f0-117">Pokud už máte Office nainstalovaný na serveru RDS pomocí jakéhokoliv jiného předplatného Microsoftu, odinstalujte ho.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="7e8f0-118">Například v **ovládacím panelu**  >  **Odinstalujte program**.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="7e8f0-119">Pokud máte problémy, odinstalujte ho pomocí nástroje [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="7e8f0-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="7e8f0-120">Na serveru RDS se přihlaste do centra pro správu Microsoft 365 s účtem správce a [nainstalujte si aplikace Microsoft 365 pro podniky](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="7e8f0-121">Po instalaci Office se ***Neotevírejte ani se přihlaste*** k žádným aplikacím Office.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="7e8f0-122">Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru pomocí následujícího postupu:</span><span class="sxs-lookup"><span data-stu-id="7e8f0-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="7e8f0-123">Klikněte pravým tlačítkem myši na tlačítko Windows v levém dolním rohu obrazovky a vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="7e8f0-124">Do pole Otevřít zadejte **Regedit**a pak vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="7e8f0-125">Když se zobrazí výzva, aby Editor registru mohl v zařízení dělat změny, vyberte **Ano** .</span><span class="sxs-lookup"><span data-stu-id="7e8f0-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="7e8f0-126">V editoru registru přidejte hodnotu řetězce **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="7e8f0-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="7e8f0-127">Na serveru RDS se ***přihlaste jako koncový uživatel*** a [Ověřte, jestli je povolená aktivace sdíleného počítače pro Microsoft 365](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="7e8f0-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

