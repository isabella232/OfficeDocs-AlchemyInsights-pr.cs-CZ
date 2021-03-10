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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693302"
---
# <a name="fix-connection-policy"></a>Oprava zásad připojení

E-mail byl označen jako bezpečný a doručený do složky doručené pošty uživatele, protože odesílající IP adresa byla v zásadách filtru připojení označená jako bezpečná. Chcete-li tyto zásady zkontrolovat, proveďte následující kroky:

1. Přejděte do Centra zabezpečení a dodržování předpisů [Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143)potom přejděte na Zásady řízení rizik – ochrana proti   >    >  [spamu.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Na kartě **Vlastní** vyberte zásadu filtru **připojení** a pak **vyberte Upravit zásadu.**
3. Zkontrolujte seznam **povolení PROTOKOLU IP.** Podívejte **se, jestli je povolený** seznam bezpečných adres.

    > [!NOTE]
    > Microsoft odebírá zdroje důvěryhodných odesílatelů od jiných výrobců. Pokud **je povolený** seznam bezpečných adres, tito důvěryhodní odesílatelé se omylem označí jako spam. Doporučujeme tuto možnost vybrat, protože se sníží počet falešně pozitivních zpráv (dobré zprávy, které jsou klasifikované jako spam), které dostanete.
