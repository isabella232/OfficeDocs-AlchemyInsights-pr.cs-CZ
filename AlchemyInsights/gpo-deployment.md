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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067833"
---
# <a name="gpo-deployment"></a>Nasazení objektu zásad skupiny

Nastavení objektů uživatelů a počítačů v Azure Active Directory Domain Services (Azure služba AD DS) se často spravují pomocí objektů Zásady skupiny (GPO). Azure služba AD DS obsahuje integrované objekty zásad skupiny pro kontejnery AADDC Users a AADDC Computers. Tyto předdefinové objekty zásad skupiny můžete přizpůsobit tak, aby zásady skupiny nakonfigurujete podle potřeby pro vaše prostředí. Členové skupiny správci Azure AD DC mají oprávnění pro správu zásad skupiny v doméně Azure služba AD DS a můžou taky vytvářet vlastní objekty zásad skupiny a organizační jednotky (OU). Další informace o tom, co jsou zásady skupiny a jak fungují, najdete v Zásady skupiny [Přehled.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

V hybridním prostředí se zásady skupiny nakonfigurované v místním služba AD DS nesynchronují s Azure služba AD DS. Pokud chcete definovat nastavení konfigurace pro uživatele nebo počítače v Azure služba AD DS, upravte jednu z výchozích objektů zásad skupiny nebo vytvořte vlastní objekt zásad skupiny.

V tomto [článku Zásady skupiny,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) jak nainstalovat nástroje pro správu Zásady skupiny, jak upravit předdefinné objekty zásad skupiny a jak vytvořit vlastní objekty zásad skupiny.
