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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329655"
---
# <a name="missing-emails-in-quarantine"></a>Chybějící e-maily v karanténě

Správci můžou tyto zprávy [zobrazit, uvolnit nebo odstranit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Na portálu Microsoft 365 Defender přejděte <https://security.microsoft.com> na **Zkontrolovat** \> **karanténu**. Pokud chcete přejít přímo na stránku **Karanténa,** použijte <https://security.microsoft.com/quarantine> .  

Další informace o hodnotách hledání a filtrování, které můžete použít, najdete v tématu Správa zpráv a souborů v karanténě jako správce v [EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Rutiny, které používáte k zobrazení a správě zpráv a souborů v karanténě, jsou:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Tato rutina je jenom pro zprávy, ne pro soubory z Sejf Přílohy pro SharePoint, OneDrive nebo Microsoft Teams.
- [Zpráva o uvolnění do karantény](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
