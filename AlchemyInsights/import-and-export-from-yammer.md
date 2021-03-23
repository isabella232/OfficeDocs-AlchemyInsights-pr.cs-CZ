---
title: Import a export z Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035091"
---
# <a name="import-and-export-from-yammer"></a>Import a export z Yammer

**Import**

Možnosti importu uživatele se liší podle toho, jestli je Yammer v nativním režimu [pro Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)nebo ne.

- **Režim,** který není nativní: Uživatele můžete importovat do skupin pomocí možnosti Přidat z adresáře [(omezit](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) na [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) 100 uživatelů) v nastavení skupiny nebo do sítě pomocí hromadné aktualizace v rámci správce sítě.
- **Nativní režim:** Operace členství ve skupině a členství v síti by se měly provádět na portálu pro správu [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [na portálu Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)nebo pomocí jiné možnosti Azure AD. Sítě v nativním režimu už nemají přístup k hromadné aktualizaci a dalším starším funkcím.

> [!IMPORTANT]
> Yammer import obsahu z správce sítě, i když byla funkce Export dat použitá v jiné síti, nikdy nepodporuje. Obsah může být znovu publikován partnerskými řešeními nebo rozhraními Yammer REST API.

**Export**

[Export síťových dat v rámci](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) správce sítě umožňuje export obsahu z Yammer, včetně zpráv a souborů. Přílohy mohou být velmi velké a způsobí, že dokončení exportu bude trvat velmi dlouho. Doporučujeme exportovat aktivní sítě pomocí rozhraní API pro [export](https://developer.yammer.com/docs/data-export-api) dat v kusech po dnech nebo týdnech. Podpora Microsoftu neposkytuje pro tento účel vlastní skripty.

Existuje samostatný [export GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) pro export obsahu pro jednotlivé uživatele.