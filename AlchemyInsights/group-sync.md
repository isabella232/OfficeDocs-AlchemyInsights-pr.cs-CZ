---
title: Synchronizace skupin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256684"
---
# <a name="group-sync"></a>Synchronizace skupin

Tento článek obsahuje pokyny k synchronizaci skupin.

1. Pokud globální správce nebo vlastník skupiny nemůže upravovat vlastnosti skupiny nebo přidávat členy nebo přiřazovat vlastníky na portálu Azure Portal, ujistěte se, že zdrojem autority pro skupinu je Azure Active Directory (Azure AD), který může globálnímu správci nebo vlastníkovi skupiny upravit skupinu.
2. Než se pokusíte odstranit synchronizované skupiny v [](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) Azure AD, ujistěte se, že jste odstranili všechny přiřazené licence, abyste se vyhnuli chybám.

Pokud chcete porozumět tomu, jak synchronizovat uživatele, skupiny a kontakty, podívejte se na Azure [AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)a sledujte synchronizaci místní skupiny s Azure pomocí Azure AD [Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) k synchronizaci místních skupin pomocí ad connect.

Postupujte podle této [příručky k řešení chyb při synchronizaci, které](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) vám pomohou vyřešit běžné chyby během synchronizace.

