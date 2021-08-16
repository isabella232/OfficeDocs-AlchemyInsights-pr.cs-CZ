---
title: Yammer problémy s licencí
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989722"
---
# <a name="yammer-licensing-issues"></a>Yammer problémy s licencí

Všichni uživatelé musí mít licenci na používání služby Yammer Enterprise, ale ve výchozím nastavení Yammer nevyžaduje, aby uživatelé museli mít licenci pro přístup ke službě. Když správce změní nastavení tak, aby Microsoft 365 uživatelům bez Yammer licencí, uživatelé, kteří nemají přiřazenou licenci Yammer Enterprise, nemají přístup ke službě Yammer. Další informace najdete v tématu [Správa Yammer uživatelských licencí v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Když jsou licence uživatelům odebrány, dlaždice Yammer se už nezobrazuje a další služby mohou pomocí odebrání licencí skrýt funkce. V ostatních případech se funkce dají pořád zobrazovat, ale vyžadují, aby licence byla k provozu.  

**Licence se uživateli ne aktualizovaná**  

Příležitostně je uživateli přiřazena licence, ale stále není schopen získat přístup k Yammer. Zpoždění jsou pravděpodobnější, když probíhá hromadné přiřazení licencí. Yammer uživatelé nemusí být aktualizováni ve stejném pořadí, ve stejném pořadí jako se změní licence v Azure AD, protože systém běží asynchronně. Počkejte až 24 hodin před otevřením případu podpory a nahlásit problémy se synchronizací licencí.  

**Hromadné přiřazení licencí**  

Licence je možné přiřadit prostřednictvím Centra pro správu nebo skriptování PowerShellu. Další informace najdete v tématu [Přiřazení licencí](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) uživatelům a Přiřazení licencí uživatelským účtům pomocí [Office 365 PowerShellu.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Podpora Microsoftu neposkytuje pomoc s vytvářením skriptů, ale je k dispozici dokumentace Yammer přiřazení licencí. Další informace najdete v tématu [Správa Yammer licencí pomocí Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).