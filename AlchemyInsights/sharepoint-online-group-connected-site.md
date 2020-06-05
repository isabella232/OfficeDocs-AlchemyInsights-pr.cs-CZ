---
title: Přidání skupiny na sharepointový web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582804"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémy při vytváření webu připojeného ke skupině v SharePointu

1. Při vytváření nebo opětovném vytváření sítě připojené skupiny došlo k některým běžným problémům.
Pokud jste odstranili skupinu a její připojený web a chcete vytvořit jiný web se stejnou adresou URL, budete muset trvale odebrat předchozí web.

   - Stažení [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Další informace o začínáme s Powershellem najdete v [tématu Začínáme s prostředím SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odeberte web z odstraněných webů pomocí [rutiny Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Prostředí Powershell je nutné trvale odstranit weby skupiny.

1. Pokud vytváříte web připojený ke skupině a zobrazí se upozornění: **Jiná skupina se stejným aliasem již existuje**, zkontrolujte existující skupiny z [Centra pro správu Microsoftu 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Chcete-li problém vyřešit, odstraňte existující skupinu, pokud již není potřeba, nebo vytvořte web s přiřazeným jiným aliasem.

1. Existují různé způsoby vytváření a používání moderních skupin pomocí SharePointu.

   - Existující weby můžete připojit ke skupině Microsoft 365. Další informace najdete v [tématu Připojení skupiny Microsoft 365 pomocí uživatelského rozhraní SharePointu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Chcete-li vytvořit propojený web skupiny Microsoft 365, budete muset vytvořit [týmový web](https://admin.microsoft.com/sharepoint).
