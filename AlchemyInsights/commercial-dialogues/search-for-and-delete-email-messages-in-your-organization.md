---
title: Hledání a odstraňování e-mailových zpráv ve vaší organizaci
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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948876"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Hledání a odstraňování e-mailových zpráv ve vaší organizaci

Postupujte takto:

1. Pokud nejste globální správce, musí být váš účet při hledání zpráv přidán do skupiny rolí **Správce eDiscovery** nebo do role správy hledání **dodržování předpisů.** Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí **Správa** organizace nebo k roli správy **Hledání a čištění.** Oprávnění k těmto rolím jsou přiřazena v [Centru & dodržování předpisů.](https://protection.office.com)
2. [Vytvořte hledání obsahu a](https://docs.microsoft.com/office365/securitycompliance/content-search) vyhledejte zprávu, kterou chcete odstranit.
3. [Připojení na Centrum & dodržování předpisů PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Pokud používáte MFA, přečtěte si tyto pokyny: [Připojení k & Compliance Center PowerShellu pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Odstranění zprávy: Spuštěním `New-ComplianceSearchAction` rutiny zprávu odstraníte. Odstraněné zprávy se přesunou do složky Obnovitelné položky uživatele. Příklad příkazu najdete v tématu [Krok 3: Odstranění zprávy.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
