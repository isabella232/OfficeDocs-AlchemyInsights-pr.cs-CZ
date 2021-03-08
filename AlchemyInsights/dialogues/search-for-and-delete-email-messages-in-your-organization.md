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
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Hledání a odstraňování e-mailových zpráv v organizaci

Postupujte takto:

1. Pokud nejste globální správce, musíte pro hledání zpráv, které váš účet přidat do skupiny rolí **správce eDiscovery** nebo do role správy vyhledávání dodržování **předpisů.** Pokud chcete odstranit zprávy, musíte se připojit ke skupině rolí Správa **organizace** nebo k roli správy vyhledávání a **vymazání.** Oprávnění k těmto rolím se přidělí v Centru zabezpečení [& dodržování předpisů.](https://protection.office.com)
2. [Vytvořte vyhledávání obsahu a](https://docs.microsoft.com/office365/securitycompliance/content-search) najděte zprávu, kterou chcete odstranit.
3. [Připojte se k & PowerShellu v Centru zabezpečení a dodržování předpisů.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Pokud používáte vícefaktorové ověřování, postupujte podle těchto pokynů: Připojení k PowerShellu & Dodržování předpisů v Centru zabezpečení [pomocí vícefaktorového ověřování](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Odstranění zprávy: Spusťte `New-ComplianceSearchAction` rutinu pro odstranění zprávy. Odstraněné zprávy se přesunou do složky uživatele Obnovitelné položky. Příklad příkazu najdete v kroku [3: Odstranění zprávy.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
