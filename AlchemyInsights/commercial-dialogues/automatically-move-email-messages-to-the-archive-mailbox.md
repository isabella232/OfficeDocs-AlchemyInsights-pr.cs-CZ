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
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059219"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatické přesunutí e-mailových zpráv do archivační poštovní schránky

Tady je postup, jak nastavit zásadu pro automatické přesunutí starého e-mailu uživatele do archivační poštovní schránky:

1. Přejděte na [**Archiv & správy**](https://go.microsoft.com/fwlink/p/?linkid=2077143)dat dodržování předpisů a ověřte, jestli je pro uživatele povolená  >    >   archivační poštovní schránka. Pokud tomu tak není,  klikněte v poli upozornění na **Povolit** a pak na Ano.
2. Přejděte do [**centra Exchange správy > dodržování předpisů > značky uchovávání informací**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Zvolte ikonu + a pak zvolte **automaticky použít pro celou poštovní schránku**.
4. Přiřaďte název značce uchovávání informací a zvolte **Přesunout do archivu**. Pro dobu uchovávání zadejte dobu, kterou chcete, například 90 dnů. Klikněte na **Uložit**.
5. Teď vytvořte zásadu uchovávání informací: zvolte zásady **uchovávání** informací , zvolte ikonu a přidejte novou zásadu.
6. Přiřaďte k zásadám uchovávání informací název, potom kliknutím a posouváním vyhledejte a přidejte značku uchovávání informací, kterou jste právě vytvořili. Klikněte na **Uložit**.
7. Nakonec použijte zásady uchovávání informací pro poštovní schránku uživatele: v Centru pro správu Exchange přejděte do **poštovních** schránek  >  **příjemců**. Vyberte všechny uživatele, u kterého chcete zásadu použít, a pak zvolte **Upravit** (ikona tužky).
8. V dialogovém okně klikněte na funkce **poštovní schránky**. V **části Zásady uchovávání** informací použijte zásadu, kterou jste právě vytvořili, > **Uložit.**
9. Pokyny k použití zásad pro všechny uživatele najdete v článku Použití zásad [uchovávání informací u poštovních schránek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
