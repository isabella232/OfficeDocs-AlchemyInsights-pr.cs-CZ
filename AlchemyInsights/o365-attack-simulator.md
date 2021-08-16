---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065277"
---
# <a name="attack-simulator-in-microsoft-365"></a>Útočný trenažér v Microsoft 365

- Chybí vám útočný trenažér? Útočný **trenažér vyžaduje Microsoft Defender pro Office 365 Plán 2** nebo Office 365 Enterprise **E5.** Attack Simulator není **součástí** programu Microsoft Defender pro Office 365 Plán 1, Office 365 Enterprise E3 nebo Microsoft 365 Apps pro firmy předplatných.

- Účet, který používáte ke spouštění simulovaných útoků, vyžaduje oprávnění globálního správce nebo správce zabezpečení a vícefaktorové ověřování (MFA). Další informace o požadavcích na útočný trenažér najdete v [tomto tématu](/microsoft-365/security/office-365-security/attack-simulator).

- Důležité informace o simulacích **útoku pomocí hesla Brute Force Password:**

  - Pokud má cílový účet povolenou vícefaktorovou ověřování a heslo bylo správně uhodnuté, účet se nebude zobrazovat jako ohrožený (druhý faktor ověřování bude neúplný).

  - Soubor hesla nemůže být větší než 10 MB. Použijte jedno heslo na řádek a za poslední heslo v seznamu zahrňte prázdný řádek (návrat k řádku).

- Důležité informace o útoku **Spear Phishing** připojte k simulacím:

  - Z návrhu nemůžete zadat vlastní hodnotu adresy **URL přihlašovacího serveru phishing.**

  - Pokud příjemce používá [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) doplněk Povolit zprávu sestavy k nahlásit zprávu jako útok phishing, nemusí se pro zprávu zobrazit upozornění (protože se jedná o simulovaný útok).

- Sestavy: Po dokončení simulovaného útoku můžete kliknout na **Podrobnosti** útoku a zobrazit tak sestavu.

- Podrobné pokyny a nové funkce v attack simulatoru najdete v článku [Útočný trenažér v Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
