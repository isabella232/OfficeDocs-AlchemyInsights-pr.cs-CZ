---
title: Chybějící e-maily v karanténě
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673707"
---
# <a name="missing-emails-in-quarantine"></a>Chybějící e-maily v karanténě

Správci můžou [tyto zprávy zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pokud chcete otevřít Centrum pro dodržování předpisů &, přejděte na [https://protection.office.com](https://protection.office.com/) . Pokud chcete stránku karantény otevřít přímo, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Můžete hledat podle následujících hodnot:  

- **ID zprávy**: globálně jedinečný identifikátor zprávy. Pokud v seznamu vyberete zprávu, zobrazí se v zobrazeném podokně informační  **seznam s**  **podrobnostmi**  . Správci můžou pomocí [sledování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) najít zprávy a odpovídající hodnoty ID zprávy.
- **E-mailová adresa odesílatele**: e-mailová adresa jednoho odesílatele
- **E-mailová adresa příjemce**: e-mailová adresa jednoho příjemce
- **Předmět**: použijte celý předmět zprávy. V hledání se nerozlišují malá a velká písmena.

Po zadání kritérií vyhledávání kliknutím na tlačítko ![ aktualizovat ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **aktualizujte** výsledky.  

K zobrazení a správě zpráv a souborů v karanténě slouží rutiny:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Náhled – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Tato rutina je jenom pro zprávy, ne pro soubory malwaru z ATP pro SharePoint Online, OneDrive pro firmy nebo týmy.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)