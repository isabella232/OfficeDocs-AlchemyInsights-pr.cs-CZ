---
title: Podmínky chybějící v úložišti termínů SharePointu Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750444"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolení šifrování nástrojem BitLocker s Intune

Zásady Endpoint Protection pro Intune se dají použít ke konfiguraci nastavení šifrování Boitlocker pro zařízení s Windows, jak je popsáno v: Windows10 (a novější) nastavení ochrany zařízení pomocí Intune.

Uvědomte si, že mnoho novějších zařízení s Windows 10 podporuje automatické šifrování BitLocker, které se spouští bez zásad MDM. To může ovlivnit použití zásad, pokud nejsou konfigurovány výchozí nastavení. Další podrobnosti najdete v častých otázkách.


Časté otázky   Q: jaké edice Windows podporují šifrování zařízení pomocí zásad ochrany koncových bodů?
 A: nastavení v Intune Endpoint Protection se implementuje pomocí CSP nástroje BitLocker.CSP nepodporují všechny edice ani buildy Windows. 
      Edice Windows: Enterprise; Podporují se vzdělávací, mobilní, mobilní a profesionální organizace (ze buildu 1809.




Otázka: Pokud je už zařízení zašifrované pomocí nástroje BitLocker s použitím výchozího nastavení OS pro metodu šifrování a šifrování (XTS-AES-128), bude se automaticky spouštět opětovné šifrování jednotky s novými nastaveními?

Odpověď: Ne. Pokud chcete použít nové nastavení šifrování, musí být jednotka nejdřív dešifrovaná.

Poznámka: u zařízení, která jsou registrovaná pomocí automatického pilotního nasazení, se automatické šifrování, ke kterému dojde při vyhodnocování zásad při spuštění, neaktivuje, dokud neproběhne vyhodnocení zásady Intune, která umožňuje použití nastavení založených na zásadách místo výchozích hodnot operačního systému.




Otázka Pokud je zařízení zašifrované v důsledku použití zásad Intune, bude při odebrání této zásady dešifrováno?

A: odebrání zásad souvisejících se šifrováním nemá za následek dešifrování nakonfigurovaných disků.




Otázka: Proč zásady pro dodržování předpisů v Intune ukazují, že moje zařízení nemá povolený nástroj BitLocker, ale je?

A: nastavení "BitLocker Enabled" v zásadách dodržování předpisů Intune využívá klienta ověření stavu zařízení s Windows (DHA). Tento klient měří pouze stav zařízení při spuštění. Takže pokud se zařízení nerestartoval po dokončení šifrování nástrojem BitLocker, klientská služba nebude nástroj BitLocker ohlásit jako aktivní.