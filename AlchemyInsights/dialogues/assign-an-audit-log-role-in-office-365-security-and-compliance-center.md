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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="7e5ca-102">Přiřazení role protokolu auditování v Centru zabezpečení a dodržování předpisů Office 365 & dodržování předpisů</span><span class="sxs-lookup"><span data-stu-id="7e5ca-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="7e5ca-103">Pokud chcete v protokolu auditování Office 365  hledat, musí mít správce přiřazenou roli Protokoly auditování jenom pro zobrazení nebo **roli** Protokoly auditování v Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7e5ca-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="7e5ca-104">Tyto role se ve výchozím nastavení přidělí skupinám rolí Správa dodržování předpisů a Správa organizace.</span><span class="sxs-lookup"><span data-stu-id="7e5ca-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="7e5ca-105">Globální správci v Office 365 a Microsoftu 365 se automaticky přidávají jako členové skupiny rolí Správa organizace.</span><span class="sxs-lookup"><span data-stu-id="7e5ca-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="7e5ca-106">Pokud chcete uživateli povolit hledání s minimální úrovní oprávnění, vytvořte vlastní skupinu rolí v Exchange Online, přidejte roli Protokoly **auditování** jenom pro zobrazení nebo roli Protokoly auditování a potom přidejte uživatele jako člena nové skupiny rolí. </span><span class="sxs-lookup"><span data-stu-id="7e5ca-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="7e5ca-107">Další informace najdete v tématu Správa skupin [rolí v Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) a Hledání protokolu auditování v Centru zabezpečení & dodržování [předpisů.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="7e5ca-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>