---
title: Chybějící e-maily v karanténě
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569049"
---
# <a name="missing-emails-in-quarantine"></a>Chybějící e-maily v karanténě"

Správci mohou [tyto zprávy zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Chcete-li otevřít Centrum dodržování zabezpečení &, přejděte na [https://protection.office.com](https://protection.office.com/) . Chcete-li přímo otevřít stránku Karanténa, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) položku .  

Vyhledávat můžete podle následujících hodnot:  

- **ID zprávy**: Globálně jedinečný identifikátor zprávy. Pokud v seznamu vyberete zprávu, zobrazí se **v** podokně informačního rámečku Podrobnosti v podokně **podrobností,** které se zobrazí. Správci mohou pomocí [trasování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) vyhledat zprávy a odpovídající hodnoty ID zprávy.
- **E-mailová adresa odesílatele**: E-mailová adresa jednoho odesílatele.
- **E-mailová adresa příjemce**: E-mailová adresa jednoho příjemce.
- **Předmět**: Použijte celý předmět zprávy. Hledání nerozeštkují malá a velká písmena.

Po zadání kritérií hledání klikněte na tlačítko Aktualizovat a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** vyfiltrujte výsledky.  

Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:
- [Odstranit-KaranténaMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-KaranténaMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Všimněte si, že tato rutina je určena pouze pro zprávy, nikoli pro soubory malwaru z ochrany ATP pro SharePoint Online, OneDrive pro firmy nebo Týmy.
- [Uvolnění-KaranténaMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)