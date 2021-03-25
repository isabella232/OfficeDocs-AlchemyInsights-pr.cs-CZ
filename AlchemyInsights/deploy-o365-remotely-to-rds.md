---
title: Nasazení aplikací Microsoft 365 pro podniky pro sdílené použití na RDS, Terminálovém serveru nebo VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200666"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="ed6ff-102">Nasazení aplikací Microsoft 365 pro podniky pro sdílené použití na RDS, Terminálovém serveru nebo VDI</span><span class="sxs-lookup"><span data-stu-id="ed6ff-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="ed6ff-103">Nasazení aplikací Microsoft 365 pro podniky pomocí služby Vzdálená plocha (RDS), dříve s názvem Terminálová služba:</span><span class="sxs-lookup"><span data-stu-id="ed6ff-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="ed6ff-104">Musíte mít plán Microsoft 365 pro firmy nebo plán Office 365, který zahrnuje Aplikace Microsoft 365 pro podniky, jako je Office 365 Enterprise E3 nebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="ed6ff-105">Plány Microsoft 365 Apps pro firmy a Microsoft 365 Business Standard nezahrnují Aplikace Microsoft 365 pro podniky.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="ed6ff-106">Musíte povolit [aktivaci sdíleného počítače](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="ed6ff-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="ed6ff-107">Můžete si taky stáhnout a spustit [Pomocníka pro](https://aka.ms/SaRA_OfficeSCA_M365Portal) podporu a obnovení Microsoftu a nainstalovat aplikace Microsoft 365 pro podniky v režimu aktivace sdíleného počítače.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="ed6ff-108">Další informace o předpokladech, pokynech k instalaci a pokynech k přizpůsobené instalaci pomocí Nástroje pro nasazení Office najdete v tématu Nasazení [aplikací Microsoft 365 pro](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)podniky pomocí služby Vzdálená plocha .</span><span class="sxs-lookup"><span data-stu-id="ed6ff-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="ed6ff-109">Oprava chyb týkajících se aktivace sdíleného počítače:</span><span class="sxs-lookup"><span data-stu-id="ed6ff-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="ed6ff-110">Podívejte [se na článek Řešení problémů s aktivací sdíleného počítače pro Aplikace Microsoft 365 pro podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="ed6ff-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="ed6ff-111">Přečtěte si téma zaměřené na [resetování stavu aktivace Microsoft 365 Apps pro podniky](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="ed6ff-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="ed6ff-112">Pokud chcete nainstalovat Microsoft 365 Apps pro podniky na RDS z Centra pro správu Microsoftu 365, které používá výchozí nastavení instalace , postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="ed6ff-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="ed6ff-113">Zkontrolujte, jaké máte předplatné.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-113">Check what subscription you have.</span></span> <span data-ttu-id="ed6ff-114">[Zjistěte, jak](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)na to.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="ed6ff-115">V případě potřeby přepněte na jiné předplatné.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="ed6ff-116">[Zjistěte, jak](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)na to.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="ed6ff-117">Pokud je Office už nainstalovaný na serveru RDS pomocí jiných předplatných Microsoftu, odinstalujte ho.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="ed6ff-118">Například tak, že v **Ovládacích panelech**  >  **odinstalujete program**.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="ed6ff-119">Pokud máte problémy, odinstalujte ji pomocí nástroje Microsoft Support and [Recovery Assistant.](https://aka.ms/SARA-OfficeUninstall-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="ed6ff-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="ed6ff-120">Na serveru RDS se přihlaste do Centra pro správu Microsoftu 365 pomocí účtu správce a [nainstalujte aplikace Microsoft 365 pro podniky](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="ed6ff-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="ed6ff-121">Po instalaci Office ***se neotev ít ani*** se přihlásit k žádným aplikacím Office.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="ed6ff-122">Na serveru RDS povolte aktivaci sdíleného počítače úpravou registru takto:</span><span class="sxs-lookup"><span data-stu-id="ed6ff-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="ed6ff-123">Klikněte pravým tlačítkem myši na tlačítko Windows v levém dolním rohu obrazovky a vyberte **Spustit.**</span><span class="sxs-lookup"><span data-stu-id="ed6ff-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="ed6ff-124">Do pole Otevřít zadejte příkaz **regedit**, a potom vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="ed6ff-125">Po **zobrazení** výzvy k povolení editoru registru k provedení změn ve vašem zařízení vyberte Ano.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="ed6ff-126">V Editoru registru přidejte řetězcovou hodnotu **SharedComputerLicensing** s nastavením 1 v části HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="ed6ff-127">Na serveru RDS se přihlaste jako koncový ***uživatel a*** ověřte, jestli je pro Aplikace [Microsoft 365 pro podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)povolená aktivace sdíleného počítače.</span><span class="sxs-lookup"><span data-stu-id="ed6ff-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
