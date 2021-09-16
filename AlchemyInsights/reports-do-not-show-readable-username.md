---
title: Sestavy v Centru pro správu Microsoftu 365 nezobrazují čitelné uživatelské jméno
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327807"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Sestavy v Centru pro správu Microsoftu 365 nezobrazují čitelné uživatelské jméno

Sestavy v Centru pro správu Microsoftu 365 nezobrazují uživatelská jména, ale místo toho zobrazují alfanumerické hodnoty, například B2BC6C15BB9FCDEA71E5CD302D228CC8.

Toto chování je očekávané a bylo oznámeno v Centru zpráv (MC275344, publikováno 3. srpna 2021). 

Globální správci můžou tuto změnu pro svého tenanta vrátit zpět a zobrazovat identifikovatelné informace o uživatelích, pokud to postupy ochrany osobních údajů dané organizace umožňují. Vrácení této změny pro tenanta:

1. V Centru pro správu přejděte na **Nastavení** > **Nastavení organizace** > [**Služby**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) a vyberte **Sestavy**. 
1. V části **Zvolte způsob zobrazování informací o uživateli** vyberte **Zobrazovat identifikovatelné informace o uživateli v sestavách** a pak sestavu znovu spusťte.