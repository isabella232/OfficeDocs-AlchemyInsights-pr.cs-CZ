---
title: Obrázek uživatele se pořád zobrazuje v Microsoft Teams organizačním diagramu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422193"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Obrázek uživatele se pořád zobrazuje v Microsoft Teams organizačním diagramu

Pokud je jedna nebo více osob ve vaší organizaci zakázané nebo odebrané a jejich profilová fotka se pořád zobrazuje v organizačním diagramu, je možné, že je nastavení **ShowInAddressLists** nastavené na False: 

1. Přejděte na Centrum pro správu Microsoftu 365 > [Aktivní uživatelé](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) a vyberte uživatele s fotkou, která se pořád zobrazuje. 
1. Vyberte kartu **Pošta** a ujistěte se, že **je možnost Zobrazit** v globálním seznamu adres nastavená na **Ne.**

Pokud nastavení **ShowInAddressLists** na **Ne** nefunguje, zkontrolujte následující: 

- Uživatel se může zobrazit v seznamu příjemců v Exchange. Další informace najdete v tématu [Správa seznamů adres v Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Uživatel se může zobrazit ze seznamu adres v Azure Active Directory. Další informace najdete v tématu [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 