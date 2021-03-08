---
title: Automatické přesunutí e-mailových zpráv do archivační poštovní schránky
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524099"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatické přesunutí e-mailových zpráv do archivační poštovní schránky

Tady je postup, jak nastavit zásadu pro automatické přesouní starých e-mailů uživatele do archivační poštovní schránky:

1. Přejděte na [**archiv & správy**](https://go.microsoft.com/fwlink/p/?linkid=2077143)dat dodržování předpisů a ověřte, jestli je pro uživatele archivační poštovní  >    >   schránka povolená. Pokud ne, klikněte v  poli upozornění na **Povolit** a Ano.
2. Přejděte do [**Centra pro správu Exchange > správy dodržování předpisů > značek uchovávání informací.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Zvolte ikonu + a pak zvolte **možnost automaticky použít pro celou poštovní schránku.**
4. Přiřaďte značku uchovávání informací a zvolte **Přesunout do archivu.** Pro dobu uchovávání informací zadejte dobu, kterou chcete, například 90 dní. Klikněte na **Uložit**.
5. Teď vytvořte zásady uchovávání informací: zvolte **zásady uchovávání** informací, zvolte ikonu a přidejte nové zásady.
6. Přiřaďte zásady uchovávání informací název a potom kliknutím a posouváním vyhledejte a přidejte značku uchovávání informací, kterou jste právě vytvořili. Klikněte na **Uložit**.
7. Nakonec použijte zásady uchovávání informací u poštovní schránky uživatele: ještě v Centru pro správu Exchange přejděte do **poštovních** schránek  >  **příjemců.** Zvolte všechny uživatele, pro které chcete zásadu použít, a pak zvolte **Upravit** (ikona tužky).
8. V dialogovém okně klikněte na funkce **poštovní schránky.** V **části Zásady uchovávání** informací použijte zásady, které jste právě vytvořili, > **Uložit.**
9. Pokyny k použití zásad u všech uživatelů najdete v tématu Použití zásad uchovávání [informací pro poštovní schránky.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
