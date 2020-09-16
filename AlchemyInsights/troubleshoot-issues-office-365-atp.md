---
title: Poradce při potížích s Office 365 Rozšířená ochrana před internetovými útoky (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758058"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="26fc9-102">Poradce při potížích s Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="26fc9-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="26fc9-103">Chcete **s doručováním e-mailových zpráv odhlášení**?</span><span class="sxs-lookup"><span data-stu-id="26fc9-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="26fc9-104">Zkuste použít možnost dynamického doručování pro zásady bezpečné přílohy ATP.</span><span class="sxs-lookup"><span data-stu-id="26fc9-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="26fc9-105">Tím se zabrání zpoždění doručení e-mailových zpráv při ochraně příjemců před škodlivými soubory.</span><span class="sxs-lookup"><span data-stu-id="26fc9-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="26fc9-106">**Chcete nahlásit falešně kladné nebo falešně záporné hodnoty**?</span><span class="sxs-lookup"><span data-stu-id="26fc9-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="26fc9-107">K odeslání souboru k analýze použijte tento odkaz: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="26fc9-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="26fc9-108">**Věděli jste, že pro e-maily poslané mezi lidmi ve vaší organizaci můžete povolit ochranu zabezpečeným odkazem ATP**.</span><span class="sxs-lookup"><span data-stu-id="26fc9-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="26fc9-109">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="26fc9-109">Follow these steps:</span></span>
    1. <span data-ttu-id="26fc9-110">Přejděte na https://protection.office.com a přihlaste se.</span><span class="sxs-lookup"><span data-stu-id="26fc9-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="26fc9-111">Přejděte na **Threat management**  >  **Policy**  >  **odkaz Bezpeční**zásady správy hrozeb.</span><span class="sxs-lookup"><span data-stu-id="26fc9-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="26fc9-112">V části **zásady, které platí pro konkrétní příjemce**, upravte (nebo přidejte) zásadu.</span><span class="sxs-lookup"><span data-stu-id="26fc9-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="26fc9-113">Vyberte **použít bezpečné odkazy na zprávy poslané v rámci organizace**.</span><span class="sxs-lookup"><span data-stu-id="26fc9-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="26fc9-114">Uložte zásady a nechte asi 30 minut, aby vaše změny fungovaly v datovém centru.</span><span class="sxs-lookup"><span data-stu-id="26fc9-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="26fc9-115">Pokud chcete získat další nápovědu ke ATP, přečtěte si článek [Office 365 – Rozšířená ochrana před internetovými útoky](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="26fc9-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>