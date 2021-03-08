---
title: Hledání a odstraňování e-mailových zpráv v organizaci
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523690"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="0ecfe-102">Hledání a odstraňování e-mailových zpráv v organizaci</span><span class="sxs-lookup"><span data-stu-id="0ecfe-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="0ecfe-103">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="0ecfe-103">Follow these steps:</span></span>

1. <span data-ttu-id="0ecfe-104">Pokud nejste globální správce, musíte pro hledání zpráv, které váš účet přidat do skupiny rolí **správce eDiscovery** nebo do role správy vyhledávání dodržování **předpisů.**</span><span class="sxs-lookup"><span data-stu-id="0ecfe-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="0ecfe-105">Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa **organizace** nebo k roli správy vyhledávání a **vymazání.**</span><span class="sxs-lookup"><span data-stu-id="0ecfe-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="0ecfe-106">Oprávnění k těmto rolím se přidělí v Centru zabezpečení [& dodržování předpisů.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="0ecfe-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="0ecfe-107">[Vytvořte vyhledávání obsahu a](https://docs.microsoft.com/office365/securitycompliance/content-search) najděte zprávu, kterou chcete odstranit.</span><span class="sxs-lookup"><span data-stu-id="0ecfe-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="0ecfe-108">[Připojte se k & PowerShellu v Centru zabezpečení a dodržování předpisů.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0ecfe-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="0ecfe-109">Pokud používáte vícefaktorové ověřování, postupujte podle těchto pokynů: Připojení k PowerShellu & Dodržování předpisů v Centru zabezpečení [pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0ecfe-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="0ecfe-110">Odstranění zprávy: Spusťte `New-ComplianceSearchAction` rutinu pro odstranění zprávy.</span><span class="sxs-lookup"><span data-stu-id="0ecfe-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="0ecfe-111">Odstraněné zprávy se přesunou do složky uživatele Obnovitelné položky.</span><span class="sxs-lookup"><span data-stu-id="0ecfe-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="0ecfe-112">Příklad příkazu najdete v kroku [3: Odstranění zprávy.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="0ecfe-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
