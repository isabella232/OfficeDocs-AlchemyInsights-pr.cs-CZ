---
title: Simulátor útoků na útoky 2681 v Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759212"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="001d5-102">Simulátor útoků na útoky v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="001d5-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="001d5-103">Postrádáte útok na útoky?</span><span class="sxs-lookup"><span data-stu-id="001d5-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="001d5-104">Simulátor útoku vyžaduje **office 365 Rozšířený plán ochrany před hrozbami 2 (ATP (plán 2)** nebo **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="001d5-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="001d5-105">Simulátor útoků na útoky **není** součástí Office 365 Rozšířený plán ochrany před hrozbami 1 (ATP – plán 1), Office 365 Enterprise E3 nebo Microsoft 365 pro firmy.</span><span class="sxs-lookup"><span data-stu-id="001d5-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="001d5-106">Účet, který používáte ke spuštění simulaci útoků, vyžaduje oprávnění globálního správce nebo správce zabezpečení a vícefaktorové ověřování (MFA).</span><span class="sxs-lookup"><span data-stu-id="001d5-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="001d5-107">Další informace o požadavcích na simulátory útoku najdete v [tomto tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="001d5-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="001d5-108">Důležité informace o simulacích útoku na útoky pomocí **hesel**</span><span class="sxs-lookup"><span data-stu-id="001d5-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="001d5-109">Pokud má cílový účet povolené MFA a heslo je správné, účet se nezobrazuje jako ohrožený (druhý ověřovací faktor nebude úplný).</span><span class="sxs-lookup"><span data-stu-id="001d5-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="001d5-110">Soubor s heslem nesmí být větší než 10 MB.</span><span class="sxs-lookup"><span data-stu-id="001d5-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="001d5-111">Na každém řádku použijte jedno heslo a za poslední heslo v seznamu zahrňte prázdný řádek.</span><span class="sxs-lookup"><span data-stu-id="001d5-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="001d5-112">Důležité informace o Spear připojení **útoků phishing** :</span><span class="sxs-lookup"><span data-stu-id="001d5-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="001d5-113">Nemůžete poskytnout vlastní hodnotu **adresy URL přihlašovacího serveru phishing**.</span><span class="sxs-lookup"><span data-stu-id="001d5-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="001d5-114">Pokud příjemce používá k nahlášení zprávy jako podvodnou [zprávu,](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) může se stát, že pro zprávu nebudete dostávat upozornění (protože jde o simulovaný útok).</span><span class="sxs-lookup"><span data-stu-id="001d5-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="001d5-115">Sestavy: po dokončení simulovaného útoku můžete sestavu zobrazit kliknutím na **Podrobnosti o útoku** .</span><span class="sxs-lookup"><span data-stu-id="001d5-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="001d5-116">Podrobné pokyny a nové funkce v simulátoru útoku najdete v tématu [simulátor útoků na útoky v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="001d5-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
