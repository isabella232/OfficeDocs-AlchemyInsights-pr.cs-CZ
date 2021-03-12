---
title: Přiřazení role Protokolu auditování v Centru zabezpečení Office 365 & dodržování předpisů
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744602"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Přiřazení role Protokolu auditování v Centru zabezpečení Office 365 & dodržování předpisů

Pokud chcete prohledat protokol auditování Office 365, musí mít správce přiřazenou roli Protokoly auditování jen pro zobrazení nebo roli **Protokoly** auditování v Exchange Online.  Tyto role jsou ve výchozím nastavení přiřazeny ke skupinám rolí Správa dodržování předpisů a Správa organizace. Globální správci v Office 365 a Microsoft 365 se automaticky přidávají jako členové skupiny rolí Správa organizace.

Pokud chcete uživateli povolit vyhledávání s minimální úrovní oprávnění, vytvořte vlastní skupinu  rolí v Exchange Online, přidejte roli Protokoly auditování jen pro zobrazení nebo Protokoly **auditování** a přidejte uživatele jako člena nové skupiny rolí.

Další informace najdete v tématu [Správa skupin](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) rolí v Exchange Online a Hledání v protokolu auditování v Centru & dodržování [předpisů](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).