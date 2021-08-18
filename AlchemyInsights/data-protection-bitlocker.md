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
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118567"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolení šifrování nástrojem BitLocker pomocí Intune

Zásady Endpoint Protection Intune se používají ke konfiguraci nastavení šifrování nástroje Bitlocker pro Windows zařízení. Další informace najdete v článku [Windows 10 (a novější)](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)k ochraně zařízení pomocí Intune.

Kromě zásad Endpoint Protection existuje také zpráva o šifrování, která poskytuje podrobnější zobrazení stavu šifrování pro zařízení. K této sestavě se dostanete z portálu MEM v části **Zařízení > Monitor a** potom v části Konfigurace vyberte Sestava [šifrování.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport) 

Pokud zjistíte, že nástroj BitLocker není povolený očekávaným způsobem nebo že profil používaný k povolení nástroje BitLocker je v chybovém stavu, přečtěte si prosím zprávu o šifrování, abyste lépe pochopili, proč k tomuto chování dochází.

Podrobnosti o tom, jak interpretovat sestavu včetně různých hodnot stavu šifrování, najdete v tématu [Sledování šifrování zařízení pomocí Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Měli byste vědět, že mnoho novějších zařízení Windows 10 podporuje automatické šifrování nástrojem BitLocker, které se aktivuje bez použití zásad MDM. Pokud je nakonfigurované jiné než výchozí nastavení, může to mít vliv na použití zásad. Další podrobnosti najdete v následujících častých otázkách.

Informace o řešení potíží s nástrojem BitLocker najdete v tématu Poradce při potížích se zásadami [nástroje BitLocker Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Nejčastější dotazy**

Otázka: Které edice Windows podporují šifrování zařízení pomocí Endpoint Protection zásad?<br>
O: Nastavení v zásadách Endpoint Protection Intune jsou implementovaná pomocí [poskytovatele kryptografických služeb nástroje BitLocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Ne všechny edice nebo buildy Windows nástroje Bitlocker csp. <br><br>

Otázka: Jak je možné nástroj BitLocker povolit na zařízeních bez nutnosti interakce s koncovým uživatelem?<br>
A: Pokud jsou splněné nezbytné předpoklady, je možné povolit nástroj BitLocker "Silent Encryption" prostřednictvím Intune. Podrobnosti o požadavcích na zařízení a nastavení příkladu zásad pro povolení tichého šifrování najdete v následujícím dokumentu: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

Otázka: Pokud už je zařízení zašifrované nástrojem BitLocker pomocí výchozího nastavení operačního systému pro metodu šifrování a sílu šifrování (XTS-AES-128), použije se při použití zásady s různým nastavením automaticky opětovné šifrování jednotky s novým nastavením?<br>
Odpověď: Ne. Pokud chcete použít nové nastavení šifrování, musí být jednotka nejdřív dešifrovaná.<br><br>
**Poznámka:** U zařízení zaregistrovaná pomocí autopilota se automatické šifrování, ke kterému došlo během OOBE, aktivuje až po vyhodnocení zásad Intune, což umožňuje použít nastavení založené na zásadách místo výchozích nastavení operačního systému.
 
Otázka: Pokud je zařízení zašifrované v důsledku použití zásad Intune, dešifruje se po odebrání této zásady?<br>
A: Odebrání zásad souvisejících se šifrováním nevedlo k dešifrování nakonfigurovaných jednotek.
 
Otázka: Proč zásady dodržování předpisů Intune ukazují, že moje zařízení nemá povolený nástroj BitLocker, i když je?<br>
A: Nastavení "Bitlocker enabled" v zásadách dodržování předpisů Intune využívá klienta DHA (Windows Device Health Attestation). Tento klient měří stav zařízení jenom při spuštění. Takže pokud se zařízení od dokončení šifrování nástrojem Bitlocker nestartuje, klientská služba DHA nebude nástroj BitLocker hlásit jako aktivní.
 
 