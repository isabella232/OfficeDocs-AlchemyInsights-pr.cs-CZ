---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731232"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolení šifrování nástrojem BitLocker s Intune

 K nastavení šifrování nástroje BitLocker pro zařízení s Windows můžete použít zásady Endpoint Protection v Intune. Další informace najdete v článku [nastavení Windows 10 (a novější), které chrání zařízení pomocí Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Uvědomte si, že mnoho novějších zařízení s Windows 10 podporuje automatické šifrování nástrojem BitLocker, které se spouští bez zásad MDM. To může ovlivnit použití zásad v případě, že nejsou nastavené výchozí nastavení. Další podrobnosti najdete v následujících nejčastějších dotazech.
 
Informace o řešení problémů s nástrojem BitLocker najdete v článku [odstraňování potíží se zásadami nástrojem BitLocker v Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Nejčastější dotazy**

 Otázka: jaké edice Windows podporují šifrování zařízení pomocí zásad ochrany koncových bodů?<br>
 A: nastavení v Intune Endpoint Protection se implementuje pomocí [CSP nástroje BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). CSP nepodporují všechny edice nebo buildy Windows. <br><br>
      V současné době jsou podporovány následující edice Windows: Enterprise, školství, Mobile, Mobile Enterprise a Professional (Build 1809 a novější).
 
Otázka: Pokud je už zařízení šifrované pomocí nástroje BitLocker s použitím výchozího nastavení OS pro metodu šifrování a složitost šifrování (XTS-AES-128), budou se při použití zásad s jinými nastaveními automaticky spouštět nové šifrování jednotky s novými nastaveními?<br>
Odpověď: Ne. Pokud chcete použít nové nastavení šifrování, musí být jednotka nejdřív dešifrovaná.<br><br>
**Poznámka:** U zařízení, která jsou registrovaná s automatickým pilotem, se automatické šifrování, které by se při spuštění předplatného spustilo, neaktivuje, dokud se nevyhodnotí zásada Intune, která umožňuje použití nastavení založených na zásadách místo výchozích hodnot operačního systému.
 
Otázka: Pokud je zařízení zašifrované v důsledku použití zásad Intune, bude při odebrání této zásady dešifrováno.<br>
A: odstranění zásad týkajících se šifrování nemá za následek dešifrování nakonfigurovaných disků.
 
Otázka: Proč nastavení zásad dodržování předpisů v Intune ukazuje, že zařízení nemá zapnutý nástroj BitLocker, i když je?<br>
A: nastavení "BitLocker Enabled" v zásadách dodržování předpisů Intune využívá klienta ověření stavu zařízení s Windows (DHA). Tento klient měří pouze stav zařízení při spuštění. Takže pokud se zařízení nerestartoval po dokončení šifrování nástrojem BitLocker, klientská služba nebude nástroj BitLocker ohlásit jako aktivní.
 
 