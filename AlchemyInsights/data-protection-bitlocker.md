---
title: DataProtection – Nástroj BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815608"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolení šifrování nástrojem BitLocker pomocí Intune

Zásady ochrany koncových bodů Intune můžete použít ke konfiguraci nastavení šifrování nástrojem Bitlocker pro zařízení s Windows. Další informace najdete v článku [Nastavení Windows 10 (a novějších)](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)k ochraně zařízení pomocí Intune .

Kromě zásad ochrany koncových bodů je k dispozici také zpráva o šifrování, která poskytuje podrobnější zobrazení stavu šifrování pro zařízení. K této sestavě se dostanete z portálu MEM v části **Zařízení > Monitor a** potom v části Konfigurace vyberte Sestava [šifrování.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport) 

Pokud zjistíte, že nástroj BitLocker není povolený očekávaným způsobem nebo že profil používaný k povolení nástroje BitLocker je v chybovém stavu, přečtěte si prosím zprávu o šifrování, abyste lépe pochopili, proč k tomuto chování dochází.

Podrobnosti o tom, jak interpretovat sestavu včetně různých hodnot stavu šifrování, najdete v tématu [Sledování šifrování zařízení pomocí Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Měli byste vědět, že mnoho novějších zařízení s Windows 10 podporuje automatické šifrování nástrojem BitLocker, které se aktivuje bez použití zásad MDM. Pokud je nakonfigurované jiné než výchozí nastavení, může to mít vliv na použití zásad. Další podrobnosti najdete v následujících častých otázkách.

Informace o řešení potíží s nástrojem BitLocker najdete v tématu [Řešení potíží se zásadami nástroje BitLocker v Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Nejčastější dotazy**

Otázka: Které edice Windows podporují šifrování zařízení pomocí zásad ochrany koncových bodů?<br>
O: Nastavení v zásadách ochrany koncových bodů Intune se implementovali pomocí [poskytovatele kryptografických služeb Nástroje bitlockeru.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Ne všechny edice nebo buildy Windows nepodporují poskytovatele kryptografických služeb bitlockeru. <br><br>

Otázka: Jak je možné nástroj BitLocker povolit na zařízeních bez nutnosti interakce s koncovým uživatelem?<br>
A: Pokud jsou splněné nezbytné předpoklady, je možné povolit nástroj BitLocker "Silent Encryption" prostřednictvím Intune. Podrobnosti o požadavcích na zařízení a nastavení příkladu zásad pro povolení tichého šifrování najdete v následujícím dokumentu: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

Otázka: Pokud už je zařízení zašifrované nástrojem BitLocker pomocí výchozího nastavení operačního systému pro metodu šifrování a sílu šifrování (XTS-AES-128), použije se při použití zásady s různým nastavením automaticky opětovné šifrování jednotky s novým nastavením?<br>
Odpověď: Ne. Pokud chcete použít nové nastavení šifrování, musí být jednotka nejdřív dešifrovaná.<br><br>
**Poznámka:** U zařízení zaregistrovaná pomocí autopilota se automatické šifrování, ke kterému došlo během OOBE, aktivuje až po vyhodnocení zásad Intune, což umožňuje použít nastavení založené na zásadách místo výchozích nastavení operačního systému.
 
Otázka: Pokud je zařízení zašifrované v důsledku použití zásad Intune, dešifruje se po odebrání této zásady?<br>
A: Odebrání zásad souvisejících se šifrováním nevedlo k dešifrování nakonfigurovaných jednotek.
 
Otázka: Proč zásady dodržování předpisů Intune ukazují, že moje zařízení nemá povolený nástroj BitLocker, i když je?<br>
A: Nastavení "Bitlocker enabled" v zásadách dodržování předpisů Intune využívá klienta DHA (Windows Device Health Attestation). Tento klient měří stav zařízení jenom při spuštění. Takže pokud se zařízení od dokončení šifrování nástrojem Bitlocker nestartuje, klientská služba DHA nebude nástroj BitLocker hlásit jako aktivní.
 
 