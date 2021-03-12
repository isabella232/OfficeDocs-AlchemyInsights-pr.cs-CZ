---
title: Office se nedaří aktivovat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704923"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="e89bc-102">Office se nedaří aktivovat</span><span class="sxs-lookup"><span data-stu-id="e89bc-102">Unable to activate Office</span></span>

- <span data-ttu-id="e89bc-103">Zkontrolujte, jestli platnost vašeho předplatného vypršela.</span><span class="sxs-lookup"><span data-stu-id="e89bc-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="e89bc-104">Ujistěte se, že máte předplatné, které umožňuje klientské licence, jako je Office 365 Business nebo Business Premium, a ověřte, že má [uživatel přiřazenou licenci.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="e89bc-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="e89bc-105">Zkontrolujte, jestli je uživatel přihlášený k Office pomocí stejného účtu, který má přiřazenou licenci.</span><span class="sxs-lookup"><span data-stu-id="e89bc-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e89bc-106">Podívejte se na [stránku stavu služeb Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) a zjistěte, jestli se vyskytly nějaké problémy.</span><span class="sxs-lookup"><span data-stu-id="e89bc-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e89bc-107">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru, jestli neblokují aplikace Microsoft 365 a přístup k internetu.</span><span class="sxs-lookup"><span data-stu-id="e89bc-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="e89bc-108">Přečtěte si [Adresy URL a rozsahy IP adres pro Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Adresy URL a rozsahy IP adres pro Office 365").</span><span class="sxs-lookup"><span data-stu-id="e89bc-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="e89bc-109">**Tip** Na počítačích s Windows za vás můžeme diagnostikovat a automaticky vyřešit několik běžných problémů s přihlášením k Office.</span><span class="sxs-lookup"><span data-stu-id="e89bc-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="e89bc-110">Pokud chcete používat náš automatizovaný nástroj, stáhněte si a spusťte nástroj **[Microsoft Support and Recovery Assistant.](https://aka.ms/SaRA-OfficeSignInScenario)**</span><span class="sxs-lookup"><span data-stu-id="e89bc-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="e89bc-111">Při řešení problémů postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="e89bc-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="e89bc-112">Otevřete aplikaci Office a [odhlaste se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) od všech existujících uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="e89bc-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e89bc-113">[Odeberte](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) a [znovu přiřaďte](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licence Office, a potom [se přihlaste k Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="e89bc-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e89bc-114">Spusťte [Poradce při potížích s aktivací](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="e89bc-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- <span data-ttu-id="e89bc-115">[Resetujte stav aktivace Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovení stavu aktivace Office").</span><span class="sxs-lookup"><span data-stu-id="e89bc-115">[Reset Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reset Office activation state")</span></span>
- <span data-ttu-id="e89bc-116">[Proveďte online opravu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA).</span><span class="sxs-lookup"><span data-stu-id="e89bc-116">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)</span></span>

<span data-ttu-id="e89bc-117">Další řešení problémů najdete tady:</span><span class="sxs-lookup"><span data-stu-id="e89bc-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="e89bc-118">Chyby typu Nelicencovaný produkt a chyby aktivace v Office</span><span class="sxs-lookup"><span data-stu-id="e89bc-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="e89bc-119">Chyba „Je nám líto, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později.“ při aktivaci Office</span><span class="sxs-lookup"><span data-stu-id="e89bc-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)