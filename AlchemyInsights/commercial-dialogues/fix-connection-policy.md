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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988081"
---
# <a name="fix-connection-policy"></a>Oprava zásad připojení

E-mail byl označený jako bezpečný a doručený do složky Doručená pošta uživatele, protože odesílající IP adresa byla v zásadách filtru připojení označená jako bezpečná. Pokud chcete zásady zkontrolovat, proveďte toto:

1. Přejděte na [Centrum Office 365 zabezpečení &](https://go.microsoft.com/fwlink/p/?linkid=2077143)dodržování předpisů a pak přejděte na Zásady správy hrozeb   >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na kartě **Vlastní** vyberte zásadu **filtru** Připojení a pak vyberte **Upravit zásadu.**
3. Zkontrolujte seznam **POVOLIT IP** adres. Podívejte se, **Sejf seznam povolený.**

    > [!NOTE]
    > Microsoft si předplatí zdroje důvěryhodných odesílatelů třetích stran. Pokud **Sejf seznam** povolený, tito důvěryhodní odesílatelé se omylem označí jako spam. Tuto možnost doporučujeme vybrat, protože se tím sníží počet falešně pozitivních zpráv (dobrá pošta, která je klasifikovaná jako spam), kterou dostanete.
