---
title: Oprava zásad tenanta (přepsání akce)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693255"
---
# <a name="fix-tenant-policy-action-override"></a>Oprava zásad tenanta (přepsání akce)

Tato zpráva se týká zásady ochrany proti nevyžádané poště ve vašem tenantovi. Chcete-li tyto zásady zkontrolovat, proveďte následující kroky:

1. Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)potom přejděte na Zásady řízení rizik – ochrana proti   >    >  [spamu.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Zkontrolujte, jestli **zdroj** zásad označuje toto:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Pokud ano, zkontrolujte **na kartě** Vlastní nastavení zásad, které zprávu ovlivnily. Je možné, že  zprávu ovlivnila standardní nastavení použitá u všech zákazníků, kteří používají Exchange Online Protection.

Další informace o konfiguraci zásad filtru spamu najdete v tématu Konfigurace zásad filtru [spamu.](https://go.microsoft.com/fwlink/?linkid=2101431)
