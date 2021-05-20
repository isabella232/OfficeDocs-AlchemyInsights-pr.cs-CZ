---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545719"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="745bc-102">Útočný trenažér v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="745bc-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="745bc-103">Chybí vám útočný trenažér?</span><span class="sxs-lookup"><span data-stu-id="745bc-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="745bc-104">Útočný **trenažér vyžaduje Microsoft Defender pro Office 365 Plán 2** nebo Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="745bc-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="745bc-105">Attack Simulator není **součástí** programu Microsoft Defender pro Office 365 Plán 1, Office 365 Enterprise E3 nebo Microsoft 365 Apps pro firmy předplatných.</span><span class="sxs-lookup"><span data-stu-id="745bc-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="745bc-106">Účet, který používáte ke spouštění simulovaných útoků, vyžaduje oprávnění globálního správce nebo správce zabezpečení a vícefaktorové ověřování (MFA).</span><span class="sxs-lookup"><span data-stu-id="745bc-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="745bc-107">Další informace o požadavcích na útočný trenažér najdete v [tomto tématu](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="745bc-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="745bc-108">Důležité informace o simulacích **útoku pomocí hesla Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="745bc-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="745bc-109">Pokud má cílový účet povolenou vícefaktorovou ověřování a heslo bylo správně uhodnuté, účet se nebude zobrazovat jako ohrožený (druhý faktor ověřování bude neúplný).</span><span class="sxs-lookup"><span data-stu-id="745bc-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="745bc-110">Soubor hesla nemůže být větší než 10 MB.</span><span class="sxs-lookup"><span data-stu-id="745bc-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="745bc-111">Použijte jedno heslo na řádek a za poslední heslo v seznamu zahrňte prázdný řádek (návrat k řádku).</span><span class="sxs-lookup"><span data-stu-id="745bc-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="745bc-112">Důležité informace o útoku **Spear Phishing** připojte k simulacím:</span><span class="sxs-lookup"><span data-stu-id="745bc-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="745bc-113">Z návrhu nemůžete zadat vlastní hodnotu adresy **URL přihlašovacího serveru phishing.**</span><span class="sxs-lookup"><span data-stu-id="745bc-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="745bc-114">Pokud příjemce používá [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) doplněk Povolit zprávu sestavy k nahlásit zprávu jako útok phishing, nemusí se pro zprávu zobrazit upozornění (protože se jedná o simulovaný útok).</span><span class="sxs-lookup"><span data-stu-id="745bc-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="745bc-115">Sestavy: Po dokončení simulovaného útoku můžete kliknout na **Podrobnosti** útoku a zobrazit tak sestavu.</span><span class="sxs-lookup"><span data-stu-id="745bc-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="745bc-116">Podrobné pokyny a nové funkce v attack simulatoru najdete v článku [Útočný trenažér v Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="745bc-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
