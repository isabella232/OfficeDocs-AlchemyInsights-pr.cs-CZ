---
title: Sestavy v Centrum pro správu Microsoftu 365 nezískatelné uživatelské jméno
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
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/04/2021
ms.locfileid: "59315870"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Sestavy v Centrum pro správu Microsoftu 365 nezískatelné uživatelské jméno

Sestavy v Centrum pro správu Microsoftu 365 neztratí uživatelská jména, ale místo toho zobrazují alfanumerické hodnoty, například B2BC6C15BB9FCDEA71E5CD302D228CC8.

Toto chování je očekávané a bylo oznámeno v Centru zpráv (MC275344, publikované 3. srpna 2021). 

Globální správci můžou tuto změnu u svého tenanta vrátit a zobrazit identifikovatelné informace o uživateli, pokud to jejich postupy ochrany osobních údajů v organizaci povolují. Pokud chcete vrátit změnu pro tenanta:

1. V Centru pro správu přejděte na **Nastavení**  >  **Nastavení organizace**  >  [**a**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)vyberte **Sestavy**. 
1. V **části Zvolte způsob zobrazení informací o uživateli** vyberte Zobrazit **identifikovatelné informace o** uživateli v sestavách a pak sestavu znovu spusťte.