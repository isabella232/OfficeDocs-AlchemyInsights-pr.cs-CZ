---
title: Termíny, které v SharePoint Online Term Store chybí
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106410"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolení šifrování nástrojem BitLocker v Intune

Zásady Endpoint Protection Intune se používají ke konfiguraci nastavení šifrování Boitlockeru pro zařízení Windows, jak je popsáno v tématu : Nastavení Windows10 (a novější) k ochraně zařízení pomocí Intune

Měli byste vědět, že mnoho novějších zařízení Windows 10 podporuje automatické šifrování bitlockeru, které se aktivuje bez použití zásad MDM. Pokud je nakonfigurované jiné než výchozí nastavení, může to mít vliv na použití zásad. Další podrobnosti najdete v častých otázkách.


Časté otázky Otázka: Které edice Windows podporují šifrování zařízení pomocí Endpoint Protection zásad?
O: Nastavení v zásadách Endpoint Protection Intune jsou implementovaná pomocí poskytovatele kryptografických služeb Nástroje bitlockeru.  Ne všechny edice ani buildy Windows podporují csP nástroje BitLocker. V tuto chvíli Windows edice: Enterprise; Podporuje se vzdělávání, mobilní Enterprise a Professional (od buildu 1809).




Otázka: Pokud už je zařízení zašifrované nástrojem BitLocker pomocí výchozího nastavení operačního systému pro metodu šifrování a sílu šifrování (XTS-AES-128), použije se zásada s různým nastavením automaticky znovu šifrování jednotky s novým nastavením?

Odpověď: Ne. Aby bylo možné použít nová nastavení šifrování, musí být jednotka nejprve dešifrována.

Poznámka: U zařízení zaregistrovaná pomocí autopilota se automatické šifrování, ke kterému došlo během OOBE, nespouštěla, dokud se nevyhodnotí zásada Intune, která umožňuje použít nastavení založené na zásadách místo výchozích nastavení operačního systému.




Otázka: Pokud je zařízení zašifrované v důsledku použití zásad Intune, dešifruje se po odebrání této zásady?

A: Odebrání zásad souvisejících se šifrováním nevedlo k dešifrování nakonfigurovaných jednotek.




Otázka: Proč zásady dodržování předpisů Intune ukazují, že moje zařízení nemá povolenou nástroj BitLocker, ale je?

A: Nastavení "Bitlocker enabled" v zásadách dodržování předpisů Intune využívá klienta DHA (Windows Device Health Attestation). Tento klient měří stav zařízení jenom při spuštění. Pokud tedy zařízení nebylo restartované od dokončení šifrování nástrojem bitlocker, klientská služba DHA nebude hlásit, že je nástroj bitlocker aktivní.