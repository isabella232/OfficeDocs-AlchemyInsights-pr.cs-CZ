---
title: Obrázek uživatele, který se nezobrazuje Microsoft Teams organizačním diagramu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792659"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Obrázek uživatele, který se nezobrazuje Microsoft Teams organizačním diagramu

Pokud jednomu nebo více jednotlivcům ve vaší organizaci v organizačním diagramu chybí jeho profilová fotka, je možné, že je nastavení **ShowInAddressLists** nastavené na **False**:

1. Přejděte na Centrum pro správu Microsoftu 365 > [**Aktivní uživatelé**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)a vyberte uživatele s chybějící fotkou. 
1. Vyberte kartu **Pošta** a ujistěte se, že je možnost Zobrazit v **globálním** seznamu adres nastavená na **Ano.** 

Pokud nastavení **ShowInAddressLists** na **Ano** nefunguje, zkontrolujte následující:

- Uživatel může být skrytý v seznamu příjemců v Exchange. Další informace najdete v tématu [Správa seznamů adres v Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Uživatel může být skrytý v seznamu adres v Azure Active Directory. Další informace najdete v tématu [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
