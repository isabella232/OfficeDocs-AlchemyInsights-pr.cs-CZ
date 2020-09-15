---
title: Řešení potíží s rozšířeným zabezpečením Office 365
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658907"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="c6218-102">Řešení potíží s rozšířeným zabezpečením Office 365</span><span class="sxs-lookup"><span data-stu-id="c6218-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="c6218-103">Zaznamenáte zpoždění doručení zpráv?</span><span class="sxs-lookup"><span data-stu-id="c6218-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="c6218-104">Použijte možnost [dynamického doručování](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v zásadě bezpečné přílohy atp.</span><span class="sxs-lookup"><span data-stu-id="c6218-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="c6218-105">Tím se zabrání zpoždění zpráv při ochraně příjemců před škodlivými soubory.</span><span class="sxs-lookup"><span data-stu-id="c6218-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="c6218-106">Chcete Microsoftu ohlásit nepravdivé kladné nebo falešně záporné hodnoty?</span><span class="sxs-lookup"><span data-stu-id="c6218-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="c6218-107">Pomocí tohoto [odkazu](https://www.microsoft.com/wdsi/filesubmission/) můžete odesílat soubory k analýze.</span><span class="sxs-lookup"><span data-stu-id="c6218-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="c6218-108">Věděli jste, že můžete povolit ochranu bezpečných odkazů pro interní e-maily poslané mezi příjemci v organizaci?</span><span class="sxs-lookup"><span data-stu-id="c6218-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="c6218-109">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="c6218-109">Follow these steps:</span></span>

  1. <span data-ttu-id="c6218-110">Přejděte na stránku [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí globálního správce nebo účtu správce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c6218-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="c6218-111">V levém navigačním podokně v části **Správa hrozeb**zvolte **Policy** \> **bezpečné odkazy**zásad.</span><span class="sxs-lookup"><span data-stu-id="c6218-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="c6218-112">V **zásadách, které platí pro celou organizaci** , vyberte zásadu a klikněte na **Upravit**.</span><span class="sxs-lookup"><span data-stu-id="c6218-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="c6218-113">V části **Nastavení**povolte **použití bezpečných odkazů na zprávy poslané v rámci organizace**.</span><span class="sxs-lookup"><span data-stu-id="c6218-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
