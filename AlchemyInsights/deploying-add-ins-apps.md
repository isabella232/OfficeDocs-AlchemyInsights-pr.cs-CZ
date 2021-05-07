---
title: Nasazení doplňků pro Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233511"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Nasazení doplňků pro Microsoft 365 Apps

Centralizované nasazení je doporučený způsob nasazení doplňků Office uživatelům a skupinám ve vaší organizaci. Pokud chcete nasadit doplňky, postupujte podle následujících kroků:

**Poznámka:** Pokud chcete nainstalovat doplňky pro Office uživatele, podívejte se na informace v tématu Zobrazení, správa a instalace doplňků v [Office aplikacích](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d). Ujistěte se také, že je povolené individuální Office doplňků pro Store. Podrobnosti najdete v tématu Zabránění stahování doplňků vypnutím Office Storu ve všech klientech [(kromě Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Zajistěte, aby vaše prostředí splňovalo požadavky na nasazení doplňků pomocí centralizovaného nasazení. Podrobnosti najdete v tématu [Požadavky](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Pokud chcete **Nastavení**  >  **doplňky,** přejděte na Microsoft 365 aplikace Získat aplikace v Centru pro  >   správu. 

Poznámky: 

- Integrované aplikace vyžadují, aby správce měl oprávnění globálního správce nebo Exchange správce.

- Při nasazování doplňků více uživatelům doporučujeme zadání provést pomocí skupin místo jednotlivých uživatelů. Podrobnosti najdete v tématu Důležité informace při přiřazování doplňku uživatelům [a skupinám.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centralizované nasazení nepodporuje uživatele ve vnořených skupinách nebo skupinách, které mají nadřazené skupiny. Podrobnosti najdete v tématu [Přiřazení uživatelů a skupin](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Ujistěte se, že je pro uživatele povolená služba správy aplikací Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a'). Podrobnosti najdete v tématu [Konfigurace vlastností aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Pokud máte problémy s nasazením doplňků pomocí integrovaných aplikací, zkuste nasazení pomocí [doplňků](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Další informace najdete tady:

[Nasazení doplňků v Centru pro správu](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Správa doplňků v Centru pro správu](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Použití rutin PowerShellu pro centralizované](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) nasazení ke správě doplňků 
 [Publikování Office pomocí Centralizovaného nasazení prostřednictvím Centra Microsoft 365 pro správu](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Poradce při potížích:](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) Uživatel neuvidí doplňky 
 [Odstraňování chyb uživatelů Office doplňky](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)