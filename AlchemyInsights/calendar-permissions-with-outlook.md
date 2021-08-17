---
title: Oprávnění kalendáře
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046097"
---
# <a name="calendar-permissions"></a>Oprávnění kalendáře

Uživatelé mohou změnit vlastní oprávnění kalendáře Outlook na webu nebo jiných klientech, ale jako správce budete možná muset také prošetřit.  
S Exchange rutiny PowerShellu se zobrazí oprávnění v kalendáři uživatele:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Další informace najdete v těchto informacích:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Oprávnění kalendáře se používají ke sdílení kalendářů, další informace o sdílení Outlook kalendáře najdete v těchto článcích:

- [Sdílení outlookového kalendáře s ostatními uživateli](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Sdílení kalendáře v Outlook na webu pro firmy](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Pokud chcete vyřešit potíže s oprávněním kalendáře, [můžete použít Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) nástroj.