---
title: Řízení přístupu k veřejným složkám pomocí Outlooku
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816733"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Řízení přístupu k veřejným složkám pomocí Outlooku

Řízení přístupu uživatelů k veřejným složkám pomocí Outlooku:

1. Použití `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Povolení přístupu uživatelů k veřejným složkám v Outlooku  
$false: Zabraňte přístupu uživatelů k veřejným složkám v Outlooku. Tato hodnota je výchozí.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Poznámka: Tento postup může řídit jenom připojení s desktopem Outlooku pro klienty s Windows. Uživatelé mohou dál přistupovat k veřejným složkám pomocí aplikace OWA nebo Outlooku pro Mac.

Další informace najdete v tématu Řízená připojení k veřejným [složkám v Outlooku.](https://aka.ms/controlpf)
