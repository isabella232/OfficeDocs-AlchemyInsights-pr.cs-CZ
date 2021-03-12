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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744477"
---
# <a name="fix-tenant-policy-action-override"></a>Oprava zásad tenanta (přepsání akce)

Tato zpráva se týká zásady ochrany proti spamu ve vašem tenantovi. Pokud chcete zásady zkontrolovat, proveďte toto:

1. Přejděte do [Centra zabezpečení Office 365 & Dodržování](https://go.microsoft.com/fwlink/p/?linkid=2077143)předpisů a pak přejděte na Zásady správy hrozeb   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Zkontrolujte, jestli **zdroj zásad** označuje následující:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Pokud ano, zkontrolujte na **kartě Vlastní** nastavení zásady, která zprávu ovlivnila. Je možné, že  zpráva ovlivnila standardní nastavení použitá pro všechny zákazníky Exchange Online Protection.

Další informace o konfiguraci zásad filtru spamu najdete v tématu [Konfigurace zásad filtru spamu](https://go.microsoft.com/fwlink/?linkid=2101431).
