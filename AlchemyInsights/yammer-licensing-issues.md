---
title: Problémy s licencováním Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148200"
---
# <a name="yammer-licensing-issues"></a>Problémy s licencováním Yammeru

Všichni uživatelé musí mít licenci k používání služby Yammer Enterprise, ale ve výchozím nastavení Yammer nevyžaduje, aby uživatelé měli licenci pro přístup ke službě. Když správce změní nastavení tak, aby blokoval uživatele Microsoft 365 bez licencí Yammeru, uživatelé, kterým není přiřazena licence Yammeru Enterprise, nemají přístup ke službě Yammer. Další informace najdete [v tématu Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Když jsou licence odebrány uživatelům, dlaždice Yammeru se už nezobrazí a ostatní služby můžou pomocí odebrání licence skrýt funkce. V ostatních případech se funkce mohou stále zobrazovat, ale vyžadují přiřazení licence k provozu.  

**Licence se pro uživatele neaktualizuje.**  

V některých příležitostech je uživateli přiřazena licence, ale stále nemůže získat přístup k Yammeru. Zpoždění je pravděpodobnější, když probíhá hromadné přiřazení licence. Uživatelé Yammeru nemusí být aktualizováni ve stejném pořadí, jako licence se mění ve službě Azure AD, protože systém běží asynchronně. Před otevřením případu podpory počkejte až 24 hodin a nahlaste problémy se synchronizací licencí.  

**Hromadné přiřazení licence**  

Licence lze přiřadit prostřednictvím centra pro správu nebo skriptování prostředí PowerShell. Další informace najdete v tématech [Přiřazení licencí uživatelům](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a Přiřazení licencí [uživatelským účtům pomocí Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Podpora společnosti Microsoft neposkytuje pomoc při vytváření skriptů, ale je k dispozici dokumentace k přiřazení licencí Yammeru. Další informace najdete v [tématu Správa licencí Yammeru pomocí prostředí Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).