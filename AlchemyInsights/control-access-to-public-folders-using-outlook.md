---
title: Řízení přístupu k veřejným složkám pomocí Outlooku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803516"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Řízení přístupu k veřejným složkám pomocí Outlooku

Řízení přístupu uživatelů k veřejným složkám v Outlooku:

1. Použití `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: povolení přístupu uživatelů k veřejným složkám v Outlooku  
$false: zabraňte přístupu uživatelů k veřejným složkám v Outlooku. Tato hodnota je výchozí.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Poznámka: Tento postup může řídit připojení pouze s desktopovou aplikací Outlook pro klienty Windows. Uživatelé mohou dál přistupovat k veřejným složkám pomocí OWA nebo Outlooku for Mac.

Další informace najdete v tématu [řízená připojení k veřejným složkám v Outlooku](https://aka.ms/controlpf) , kde najdete další informace.
