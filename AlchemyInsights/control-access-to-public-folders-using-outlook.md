---
title: Řízení přístupu k veřejným složkám pomocí Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032551"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Řízení přístupu k veřejným složkám pomocí Outlook

Řízení přístupu uživatelů k veřejným složkám pomocí Outlook:

1. Použití `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Povolení přístupu uživatelů k veřejným složkám v Outlook  
$false: Zabraňte přístupu uživatelů k veřejným složkám v Outlook. Tato hodnota je výchozí.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Poznámka: Tento postup může řídit připojení jenom Outlook plochy pro Windows klienty. Uživatelé mohou dál přistupovat k veřejným složkám pomocí OWA nebo Outlook pro Mac.

Další informace najdete v tématu [Řízená připojení k](https://aka.ms/controlpf) veřejným složkám v Outlook další informace.
