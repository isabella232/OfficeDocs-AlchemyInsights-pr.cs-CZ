---
title: Nasazení objektu zásad skupiny
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427087"
---
# <a name="gpo-deployment"></a>Nasazení objektu zásad skupiny

Nastavení pro objekty uživatelů a počítačů v Azure služba Active Directory Domain Services (Azure služba AD DS) se často spravují pomocí Zásady skupiny objektů (GPOs). Azure služba AD DS obsahuje integrované gpOs pro uživatele AADDC a kontejnery AADDC Computers. Tyto předdefinové gpOs můžete přizpůsobit a konfigurovat zásady skupiny podle potřeby ve vašem prostředí. Členové skupiny správců Azure AD DC mají oprávnění pro správu zásad skupiny v doméně Azure služba AD DS a můžou taky vytvářet vlastní GPO a organizační jednotky. Další informace o zásadách skupiny a o tom, jak fungují, najdete v [Zásady skupiny přehledu.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

V hybridním prostředí se zásady skupiny nakonfigurované v místním služba AD DS nesynchronují s Azure služba AD DS. Pokud chcete definovat nastavení konfigurace pro uživatele nebo počítače v Azure služba AD DS, upravte jednu z výchozích zásad skupiny zásad skupiny nebo vytvořte vlastní objekt zásad skupiny.

V tomto [článku se Zásady skupiny,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) jak nainstalovat nástroje pro správu Zásady skupiny, jak upravit integrované gpOs a jak vytvářet vlastní GPO.
