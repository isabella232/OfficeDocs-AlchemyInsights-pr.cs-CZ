---
title: Problémy s licencováním Yammeru
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657269"
---
# <a name="yammer-licensing-issues"></a>Problémy s licencováním Yammeru

Všichni uživatelé musí mít licenci k používání služby Yammer Enterprise, ale ve výchozím nastavení Yammeru nevyžadují, aby uživatelé měli licenci pro přístup ke službě. Když správce změní nastavení tak, aby blokoval uživatele Microsoft 365 bez licencí na Yammeru, uživatelé, kteří nemají přiřazenou licenci Yammeru Enterprise, nemají přístup ke službě Yammer. Další informace najdete v tématu [Správa uživatelských licencí Yammeru v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) . 

Po odebrání licencí uživatelům se dlaždice Yammeru už nezobrazuje a další služby můžou pomocí odebrání licence tyto funkce skrýt. V ostatních případech se funkce mohou stále zobrazovat, ale vyžadují, aby fungovaly.  

**Licence není pro uživatele aktualizovaná**  

Uživateli je příležitostně přiřazena licence, ale stále neumožňuje přístup k Yammeru. Prodleva se pravděpodobněji projeví při přiřazování hromadných licencí. Uživatelé Yammeru se nemusí aktualizovat ve stejném pořadí, protože se v Azure AD změní licence, protože systém běží asynchronně. Počkejte až 24 hodin před otevřením případu podpory k nahlášení problémů se synchronizací licencí.  

**Hromadné přidělování licencí**  

Licence se dají přiřadit prostřednictvím centra pro správu nebo skriptování PowerShellu. Další informace najdete v článku [přiřazení licencí uživatelům](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a [přiřazení licencí uživatelským účtům pomocí Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Podpora Microsoftu neposkytuje pomoc při vytváření skriptů, ale k dispozici je dokumentace k přiřazení licencí Yammeru. Další informace najdete v tématu [Správa licencí Yammeru pomocí Windows PowerShellu](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).