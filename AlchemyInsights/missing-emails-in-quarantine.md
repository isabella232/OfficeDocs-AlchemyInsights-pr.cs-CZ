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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539817"
---
# <a name="missing-emails-in-quarantine"></a>Chybějící e-maily v karanténě"

Správci [můžou tyto zprávy zobrazit, uvolnit nebo odstranit.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Pokud chcete otevřít Centrum & dodržování předpisů, přejděte na [https://protection.office.com](https://protection.office.com/) . Pokud chcete stránku Karanténa otevřít přímo, přejděte na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Můžete hledat podle následujících hodnot:  

- **ID zprávy:** Globálně jedinečný identifikátor zprávy. Pokud v seznamu vyberete zprávu, zobrazí se **hodnota ID zprávy** v podokně podrobností, které se zobrazí.  Správci mohou pomocí [sledování zpráv](/microsoft-365/security/office-365-security/message-trace-scc) najít zprávy a odpovídající hodnoty ID zprávy.
- **E-mailová adresa** odesílatele: E-mailová adresa jednoho odesílatele.
- **E-mailová adresa příjemce:** E-mailová adresa jednoho příjemce.
- **Předmět:** Použijte celý předmět zprávy. Při hledání se rozlišují malá a velká písmena.

Po zadání kritérií hledání klikněte na tlačítko Aktualizovat aktualizovat a ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  vyfiltrujte výsledky.

Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Tato rutina je jenom pro zprávy, ne pro soubory malwaru z programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive pro firmy nebo Teams.
- [Zpráva o uvolnění do karantény](/powershell/module/exchange/release-quarantinemessage)