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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892040"
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
