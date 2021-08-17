---
title: Oprava zásad připojení
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314837"
---
# <a name="fix-connection-policy"></a>Oprava zásad připojení

E-mail byl označený jako bezpečný a doručený do složky Doručená pošta uživatele, protože zdrojová IP adresa byla ve výchozí zásadách filtru připojení označena jako bezpečná. Pokud chcete zásady zkontrolovat, postupujte takto:

1. Na portálu Microsoft 365 Defender na webu přejděte na E-mail & zásady spolupráce & pravidla zásady hrozeb <https://security.microsoft.com/>  \>  \>  \> **Anti-spam** v **části Zásady.**

   Pokud chcete přejít přímo na stránku Zásady ochrany **proti spamu,** použijte <https://security.microsoft.com/antispam> .

2. Na stránce **Zásady ochrany proti spamu** vyberte zásadu s názvem Zásada filtru **připojení (výchozí)** kliknutím na název zásady.

3. V okně podrobností, který se zobrazí, klikněte **v** části Filtrování připojení na Upravit zásadu **filtru** připojení.

4. Zkontrolujte položky v části Vždy **povolit zprávy** z následující IP adresy nebo rozsah adres a podívejte se, jestli **je zaškrtnuté políčko Zapnout bezpečný** seznam.

   **Poznámka:** Microsoft se přihlásí k odběru zdrojů důvěryhodných odesílatelů od jiných výrobců. Pokud je povolený bezpečný seznam, tito důvěryhodní odesílatelé nejsou omylem označeni jako spam. Tuto možnost doporučujeme vybrat, protože se sníží počet falešně pozitivních zpráv (dobrá pošta, která je klasifikovaná jako spam), kterou dostanete.

Další informace najdete v tématu [Konfigurace filtrování připojení](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
