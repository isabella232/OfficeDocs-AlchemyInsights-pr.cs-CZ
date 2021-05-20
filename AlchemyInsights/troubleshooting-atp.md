---
title: Řešení potíží s aplikací Microsoft Defender pro Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545261"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="01cd5-102">Řešení potíží s aplikací Microsoft Defender pro Office 365</span><span class="sxs-lookup"><span data-stu-id="01cd5-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="01cd5-103">**Všimli jste si zpoždění při doručování zpráv?**</span><span class="sxs-lookup"><span data-stu-id="01cd5-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="01cd5-104">Pomocí možnosti [Dynamické doručování](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v programu Microsoft Defender můžete použít Office 365 přílohy.</span><span class="sxs-lookup"><span data-stu-id="01cd5-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="01cd5-105">To pomůže zabránit zpoždění zpráv při ochraně příjemců před škodlivými soubory.</span><span class="sxs-lookup"><span data-stu-id="01cd5-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="01cd5-106">**Chcete Microsoftu nahlásit falešná kladná nebo falešná negativa?**</span><span class="sxs-lookup"><span data-stu-id="01cd5-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="01cd5-107">Použijte [Průzkumníka odeslání.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="01cd5-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="01cd5-108">-\*\* Věděli jste, že můžete povolit ochranu bezpečných odkazů pro interní e-maily odeslané mezi příjemci ve vaší organizaci?\*\* Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="01cd5-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="01cd5-109">Přejděte na účet globálního správce nebo správce [https://protection.office.com](https://protection.office.com) zabezpečení a přihlaste se.</span><span class="sxs-lookup"><span data-stu-id="01cd5-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="01cd5-110">V levém navigačním podokně v části **Správa hrozeb** zvolte **Bezpečné** \> **odkazy zásad**.</span><span class="sxs-lookup"><span data-stu-id="01cd5-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="01cd5-111">V části **Zásady, které platí pro celou** organizaci, vyberte zásadu a klikněte na **Upravit.**</span><span class="sxs-lookup"><span data-stu-id="01cd5-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="01cd5-112">V **Nastavení** povolte **Použít bezpečné odkazy na zprávy odeslané v organizaci**.</span><span class="sxs-lookup"><span data-stu-id="01cd5-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
