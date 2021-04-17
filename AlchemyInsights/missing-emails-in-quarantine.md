---
title: Chybějící e-maily v karanténě
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831727"
---
# <a name="missing-emails-in-quarantine"></a>Chybějící e-maily v karanténě"

Správci [můžou tyto zprávy zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Pokud chcete otevřít Centrum & dodržování předpisů, přejděte na [https://protection.office.com](https://protection.office.com/) . Pokud chcete stránku Karanténa otevřít přímo, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Můžete hledat podle následujících hodnot:  

- **ID zprávy:** Globálně jedinečný identifikátor zprávy. Pokud v seznamu vyberete zprávu, zobrazí se **hodnota ID zprávy** v podokně podrobností, které se zobrazí.  Správci mohou pomocí [sledování zpráv](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) najít zprávy a odpovídající hodnoty ID zprávy.
- **E-mailová adresa** odesílatele: E-mailová adresa jednoho odesílatele.
- **E-mailová adresa příjemce:** E-mailová adresa jednoho příjemce.
- **Předmět:** Použijte celý předmět zprávy. Při hledání se rozlišují malá a velká písmena.

Po zadání kritérií hledání klikněte na tlačítko Aktualizovat aktualizovat a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  vyfiltrujte výsledky.  

Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Tato rutina je jenom pro zprávy, ne pro soubory malwaru z atp pro SharePoint Online, OneDrive pro firmy nebo Teams.
- [Zpráva o uvolnění do karantény](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)