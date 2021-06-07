---
title: Nelze aktivovat Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798673"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="81427-102">Nelze aktivovat Office</span><span class="sxs-lookup"><span data-stu-id="81427-102">Unable to activate Office</span></span>

<span data-ttu-id="81427-103">**Poznámka:** Pokud používáte starší verzi Windows (například Windows 7), ujistěte se, že je jako výchozí povolená tls 1.2.</span><span class="sxs-lookup"><span data-stu-id="81427-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="81427-104">Další informace najdete v článku Aktualizace a povolení [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako výchozích zabezpečených protokolů ve WinHTTP v Windows .</span><span class="sxs-lookup"><span data-stu-id="81427-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="81427-105">Zkontrolujte, jestli platnost vašeho předplatného vypršela.</span><span class="sxs-lookup"><span data-stu-id="81427-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="81427-106">Ujistěte se, že máte předplatné, které umožňuje klientské licence, například Office 365 Business nebo obchodní Premium, a zkontrolujte, jestli má [uživatel přiřazenou licenci.](/microsoft-365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="81427-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="81427-107">Zkontrolujte, jestli je uživatel přihlášený k Office pomocí stejného účtu, který má přiřazenou licenci.</span><span class="sxs-lookup"><span data-stu-id="81427-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="81427-108">Podívejte se na [stránku stavu služeb Office 365](/office365/enterprise/view-service-health) a zjistěte, jestli se vyskytly nějaké problémy.</span><span class="sxs-lookup"><span data-stu-id="81427-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="81427-109">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že Microsoft 365 aplikace neblokují přístup k internetu.</span><span class="sxs-lookup"><span data-stu-id="81427-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="81427-110">Přečtěte si [Adresy URL a rozsahy IP adres pro Office 365](/office365/enterprise/urls-and-ip-address-ranges "Rozsahy adres IP a URL Office 365.").</span><span class="sxs-lookup"><span data-stu-id="81427-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="81427-111">**Tip** Na Windows počítačích můžeme diagnostikovat a automaticky opravit několik běžných problémů Office přihlášení.</span><span class="sxs-lookup"><span data-stu-id="81427-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="81427-112">Stáhněte si a spusťte **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** a použijte náš automatizovaný nástroj.</span><span class="sxs-lookup"><span data-stu-id="81427-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="81427-113">Při řešení problémů postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="81427-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="81427-114">Otevřete aplikaci Office a [odhlaste se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) od všech existujících uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="81427-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="81427-115">[Odeberte](/microsoft-365/admin/manage/remove-licenses-from-users) a [znovu přiřaďte](/microsoft-365/admin/manage/assign-licenses-to-users) licence Office, a potom [se přihlaste k Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí ovlivněného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="81427-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="81427-116">Spusťte [Poradce při potížích s aktivací](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="81427-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- <span data-ttu-id="81427-117">[Resetujte stav aktivace Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovení Office stavu aktivace").</span><span class="sxs-lookup"><span data-stu-id="81427-117">[Reset Office activation state](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reset Office activation state")</span></span>
- <span data-ttu-id="81427-118">[Proveďte online opravu Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA).</span><span class="sxs-lookup"><span data-stu-id="81427-118">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)</span></span>

<span data-ttu-id="81427-119">Další řešení problémů najdete tady:</span><span class="sxs-lookup"><span data-stu-id="81427-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="81427-120">Chyby typu Nelicencovaný produkt a chyby aktivace v Office</span><span class="sxs-lookup"><span data-stu-id="81427-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="81427-121">Chyba „Je nám líto, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později.“ při aktivaci Office</span><span class="sxs-lookup"><span data-stu-id="81427-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)