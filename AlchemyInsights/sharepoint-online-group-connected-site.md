---
title: Přidání skupiny na SharePoint webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093666"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Běžné problémy při vytváření webu připojeného ke skupině v SharePoint

1. Pokud jste odstranili skupinu a její připojený web a chcete vytvořit jiný web se stejnou adresou URL, budete muset předchozí web trvale odebrat.

   - Stažení [prostředí SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Další informace o tom, jak začít pracovat s PowerShellem, najdete v článku Začínáme [s SharePoint Online Management Shell](/powershell/module/sharepoint-online/remove-sposite).
   - Odeberte web z odstraněných webů pomocí [rutiny Powershellu Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell je nutný k trvalému odstranění webů skupin.

1. Pokud vytváříte web připojený ke skupině a zobrazí se upozornění: Jiná skupina se stejným **aliasem** už existuje , zkontrolujte existující skupiny z [Centrum pro správu Microsoftu 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Pokud chcete tento problém vyřešit, odstraňte existující skupinu, pokud už není potřeba, nebo vytvořte web s přiřazeným jiným aliasem.

1. Existují různé způsoby, jak vytvářet a používat moderní skupiny s SharePoint.

   - Existující weby můžete připojit ke Microsoft 365 skupině. Další informace najdete v [Připojení Microsoft 365 skupiny pomocí SharePoint rozhraní](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Pokud chcete Microsoft 365 web připojený ke skupině, musíte vytvořit [týmový web](https://admin.microsoft.com/sharepoint).
