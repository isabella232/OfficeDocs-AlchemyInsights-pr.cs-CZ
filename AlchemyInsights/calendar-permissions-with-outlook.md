---
title: Oprávnění ke kalendáři
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748786"
---
# <a name="calendar-permissions"></a>Oprávnění ke kalendáři

Uživatelé mohou změnit svá vlastní oprávnění ke kalendáři v Outlooku na webu nebo na jiných klientech, ale jako správce, který bude pravděpodobně nutné zkontrolovat.  
Pomocí rutiny Exchange PowerShellu se zobrazí oprávnění pro kalendář uživatele:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Další informace najdete v těchto tématech:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Oprávnění ke kalendáři: používá se při sdílení kalendářů. Další informace o sdílení kalendáře Outlooku najdete v těchto článcích:

- [Sdílení outlookového kalendáře s ostatními uživateli](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Sdílení kalendáře v Outlooku na webu pro firmy](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Pokud chcete vyřešit problém s oprávněním kalendáře, můžete použít nástroj [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .