---
title: Řešení chyb nelicencovaných produktů
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737946"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="c4070-102">Návrhy na řešení potíží s chybami "nelicencovaný produkt"</span><span class="sxs-lookup"><span data-stu-id="c4070-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="c4070-103">Chcete-li vyřešit chyby týkající se "nelicencovaný produkt", vyzkoušejte následující postup:</span><span class="sxs-lookup"><span data-stu-id="c4070-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="c4070-104">Zkontrolujte, jestli vypršela platnost vašeho předplatného.</span><span class="sxs-lookup"><span data-stu-id="c4070-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="c4070-105">Zkontrolujte, že máte předplatné, které umožňuje klientské licence, jako jsou aplikace Microsoft 365 pro firmy nebo Business Premium, a [zajistěte, aby byl uživateli přiřazená licence](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="c4070-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="c4070-106">Ujistěte se, že se uživatel přihlašuje k Office pomocí stejného účtu, který má přiřazenou licenci.</span><span class="sxs-lookup"><span data-stu-id="c4070-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="c4070-107">Na [stránce stavu služeb](https://docs.microsoft.com/office365/enterprise/view-service-health) se podívejte, jestli existují nějaké problémy se službou.</span><span class="sxs-lookup"><span data-stu-id="c4070-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="c4070-108">Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru, abyste ověřili, že neblokují aplikace Microsoft 365 přístup k Internetu.</span><span class="sxs-lookup"><span data-stu-id="c4070-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="c4070-109">Podívejte [se na adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="c4070-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="c4070-110">Můžete se taky pokusit o následující akce řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="c4070-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="c4070-111">Otevřete aplikaci Office a [odhlaste](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se z existujících uživatelských účtů.</span><span class="sxs-lookup"><span data-stu-id="c4070-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="c4070-112">[Odeberte](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) a [znovu přiřaďte](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenci Office a pak se [přihlaste k Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocí příslušného uživatelského účtu.</span><span class="sxs-lookup"><span data-stu-id="c4070-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="c4070-113">Spusťte [Poradce při potížích s aktivací](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="c4070-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="c4070-114">[Resetujte stav aktivace Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="c4070-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="c4070-115">[Provedení online opravy Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="c4070-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="c4070-116">Další řešení problémů najdete tady:</span><span class="sxs-lookup"><span data-stu-id="c4070-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="c4070-117">Chyby typu Nelicencovaný produkt a chyby aktivace v Office</span><span class="sxs-lookup"><span data-stu-id="c4070-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="c4070-118">Chyba „Je nám líto, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později.“ při aktivaci Office</span><span class="sxs-lookup"><span data-stu-id="c4070-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)