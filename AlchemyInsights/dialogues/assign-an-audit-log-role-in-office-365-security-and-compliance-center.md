---
title: Přiřazení role protokolu auditování v Centru zabezpečení a dodržování předpisů Office 365 & dodržování předpisů
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523972"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Přiřazení role protokolu auditování v Centru zabezpečení a dodržování předpisů Office 365 & dodržování předpisů

Pokud chcete v protokolu auditování Office 365  hledat, musí mít správce přiřazenou roli Protokoly auditování jenom pro zobrazení nebo **roli** Protokoly auditování v Exchange Online. Tyto role se ve výchozím nastavení přidělí skupinám rolí Správa dodržování předpisů a Správa organizace. Globální správci v Office 365 a Microsoftu 365 se automaticky přidávají jako členové skupiny rolí Správa organizace.

Pokud chcete uživateli povolit hledání s minimální úrovní oprávnění, vytvořte vlastní skupinu rolí v Exchange Online, přidejte roli Protokoly **auditování** jenom pro zobrazení nebo roli Protokoly auditování a potom přidejte uživatele jako člena nové skupiny rolí. 

Další informace najdete v tématu Správa skupin [rolí v Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) a Hledání protokolu auditování v Centru zabezpečení & dodržování [předpisů.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)