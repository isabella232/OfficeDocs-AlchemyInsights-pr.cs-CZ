---
title: Zjištění problémů s virtuálním desktopem Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595512"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Zjištění problémů s virtuálním desktopem Windows

Windows Virtual Desktop Diagnostics používá jenom jednu rutinu PowerShellu, ale obsahuje mnoho volitelných parametrů, které pomáhají zúžit a izolovat problémy. Začínáme: 

1. Stáhněte a naimportujte modul Windows Virtual Desktop PowerShell. Podrobnosti najdete v tématu [Rutiny virtuální plochy Windows pro Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Přihlaste se ke svému účtu spuštěním následující rutiny:
    
    Příklad: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**POZNÁMKA:** Všechny dotazy používající PowerShell musí obsahovat parametry -UserName nebo -ActivityID. Informace o možnostech monitorování najdete v tématu Použití [analýzy protokolů pro funkci diagnostiky.](https://go.microsoft.com/fwlink/?linkid=2126847)

Pokud chcete filtrovat diagnostické aktivity podle uživatele, spusťte následující rutinu:

Příklad: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Existuje seznam filtrů, které můžete spustit, abyste diagnostikovali problémy. Další informace o diagnostice problémů najdete v tématu Určení a diagnostika problémů s [virtuálním desktopem Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Další informace o běžných chybách najdete v tématu [Běžné chyby senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
