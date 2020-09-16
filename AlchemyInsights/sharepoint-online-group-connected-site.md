---
title: Přidání skupiny na web služby SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771192"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémy při vytváření skupinového propojeného webu na SharePointu

1. Vyskytly se některé běžné problémy při vytváření nebo opětovném vytváření skupinového propojeného webu.
Pokud jste odstranili skupinu a její připojený web a chcete vytvořit další web se stejnou adresou URL, budete muset trvale odebrat předchozí Web.

   - Stáhnout [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Další informace o úvodním prostředí PowerShellu najdete v tématu [Začínáme se službou SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odeberte web z odstraněných webů pomocí rutiny [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. K trvalému odstranění skupinových webů je potřeba PowerShell.

1. Pokud vytváříte web připojený ke skupině a dostanete upozornění: **už existuje jiná skupina se stejným aliasem**, podívejte se na existující skupiny v centru pro [správu Microsoftu 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Tento problém vyřešíte tak, že odstraníte existující skupinu, pokud ji už nepotřebujete nebo pokud chcete vytvořit web s jiným přiřazeným aliasem.

1. Moderní skupiny se SharePointem můžete vytvářet a používat různými způsoby.

   - Existující weby můžete připojit ke skupině Microsoft 365. Další informace najdete v článku [připojení skupiny Microsoft 365 pomocí uživatelského rozhraní SharePointu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Pokud chcete vytvořit web s připojenou skupinou Microsoft 365, budete muset vytvořit [týmový web](https://admin.microsoft.com/sharepoint).
