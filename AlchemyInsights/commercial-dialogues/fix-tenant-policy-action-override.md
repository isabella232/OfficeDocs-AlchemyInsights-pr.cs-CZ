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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326790"
---
# <a name="fix-tenant-policy-action-override"></a>Oprava zásad tenanta (přepsání akce)

Tato zpráva se týká jedné z vašich zásad ochrany proti spamu. Pokud chcete zkontrolovat zásady, postupujte takto:

1. Na portálu Microsoft 365 Defender na webu přejděte na E-mail & zásady spolupráce & pravidla zásady hrozeb <https://security.microsoft.com/>  \>  \>  \> **Anti-spam** v **části Zásady.**

   Pokud chcete přejít přímo na stránku Zásady ochrany **proti spamu,** použijte <https://security.microsoft.com/antispam> .

2. Na **stránce Anti-spam policies** (Zásady ochrany proti spamu) vyberte  zásadu kliknutím na  název zásady (**Typ** je Vlastní zásada ochrany proti spamu nebo Název je zásada příchozí pošty **antispamové pošty (výchozí).**
3. V plovoucím seznamu podrobností, který se zobrazí, **vyberte v** části **Akce** možnost Upravit akce.
4. V části Akce **zprávy** si projděte výroky spamu **,** spamu s vysokou spolehlivostí, phishingu a phishingu s vysokou spolehlivostí a zkontrolujte, jestli je vybraná kterákoli z následujících hodnot:  
   - **Přidání záhlaví X**
   - **Předpřipravené předměty s textem**
   - **Přesměrovat zprávu na e-mailovou adresu**
   - **Odstranit zprávu**
   - **Žádná akce**

   Je možné, že standardní nastavení použité **u** všech Exchange Online Protection zákazníci zprávu ovlivnili.

Další informace najdete v tématu [Konfigurace zásad ochrany proti spamu v programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
