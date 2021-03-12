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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744849"
---
# <a name="fix-connection-policy"></a>Oprava zásad připojení

E-mail byl označený jako bezpečný a doručený do složky Doručená pošta uživatele, protože odesílající IP adresa byla v zásadách filtru připojení označená jako bezpečná. Pokud chcete zásady zkontrolovat, proveďte toto:

1. Přejděte do [Centra zabezpečení Office 365 & Dodržování](https://go.microsoft.com/fwlink/p/?linkid=2077143)předpisů a pak přejděte na Zásady správy hrozeb   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na kartě **Vlastní** vyberte zásadu **filtru** Připojení a pak vyberte **Upravit zásadu.**
3. Zkontrolujte seznam **POVOLIT IP** adres. Podívejte se, **jestli je povolený** bezpečný seznam.

    > [!NOTE]
    > Microsoft si předplatí zdroje důvěryhodných odesílatelů třetích stran. Pokud **je povolený** bezpečný seznam, tito důvěryhodní odesílatelé se omylem označí jako spam. Tuto možnost doporučujeme vybrat, protože se tím sníží počet falešně pozitivních zpráv (dobrá pošta, která je klasifikovaná jako spam), kterou dostanete.
