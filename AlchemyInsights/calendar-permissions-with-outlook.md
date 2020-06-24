---
title: Oprávnění kalendáře
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862060"
---
# <a name="calendar-permissions"></a>Oprávnění kalendáře

Uživatelé mohou změnit svá vlastní oprávnění kalendáře s aplikací Outlook na webu nebo jiných klientech, ale jako správce možná budete muset také prozkoumat.  
S exchange PowerShell rutina vám ukáže oprávnění v kalendáři uživatele:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Další informace naleznete v následujících tématech:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Nastavení složky poštovní schránkyPermie](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Oprávnění kalendáře se používají při sdílení kalendářů, chcete-li zobrazit další informace o sdílení kalendáře aplikace Outlook, přečtěte si tyto články:

- [Sdílení outlookového kalendáře s ostatními uživateli](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Sdílení kalendáře v Outlooku na webu pro firmy](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Při odstraňování potíží s oprávněním kalendáře můžete použít nástroj [Pomocník pro podporu a obnovení.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)