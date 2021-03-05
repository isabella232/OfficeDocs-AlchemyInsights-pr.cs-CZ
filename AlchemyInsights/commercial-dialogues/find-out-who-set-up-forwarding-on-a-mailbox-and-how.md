---
title: Zjistěte, kdo nastaví přeposílání v poštovní schránce a jak
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481203"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Zjistěte, kdo nastaví přeposílání v poštovní schránce a jak

Pokud bylo u poštovní schránky nastavené externí přeposílání, aktivita se audituje jako součást rutiny Set-Mailbox Serveru. Tady je postup, jak najít aktivitu v protokolu auditování:

1. Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 & dodržování předpisů.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vyberte **Hledat v** protokolu >  **auditování.**
    > [!NOTE]
    > Pokud vidíte oznámení, že je potřeba auditování zapnout, můžete ho teď zapnout. Pokud tato funkce není zapnutá, výsledky hledání nebudou moct natahovat data z předchozích dat.
1. Ujistěte **se, že** je v poli Aktivity nastavené zobrazení **výsledků pro všechny aktivity** (výchozí nastavení). Zadejte rozsah dat. Nemusíte zazadat uživatelské jméno.
1. Vyberte **Hledat.** Aktivity se zobrazí v části **Výsledky.**
1. Vyberte **Výsledky filtru a** potom do  pole Filtru aktivity zadejte Nastavit poštovní schránku.  Vrátí všechny **aktivity nastavené poštovní schránky.**
1. Pokud chcete zobrazit podrobnosti, vyberte aktivitu a pak **vyberte Další informace.** V **části Parametry** můžete vidět e-mailovou adresu pro přeposílání nastavenou v poštovní schránce. ID **uživatele** představuje uživatele, který u poštovní schránky nastavil externí přeposílání.
Další informace najdete v protokolu [auditování Office 365,](https://go.microsoft.com/fwlink/?linkid=2103944)kde najdete řešení běžných scénářů.