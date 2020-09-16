---
title: Simulátor útoků na útoky 2681 v Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759212"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulátor útoků na útoky v Microsoft 365

- Postrádáte útok na útoky? Simulátor útoku vyžaduje **office 365 Rozšířený plán ochrany před hrozbami 2 (ATP (plán 2)** nebo **Office 365 Enterprise E5**. Simulátor útoků na útoky **není** součástí Office 365 Rozšířený plán ochrany před hrozbami 1 (ATP – plán 1), Office 365 Enterprise E3 nebo Microsoft 365 pro firmy.

- Účet, který používáte ke spuštění simulaci útoků, vyžaduje oprávnění globálního správce nebo správce zabezpečení a vícefaktorové ověřování (MFA). Další informace o požadavcích na simulátory útoku najdete v [tomto tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Důležité informace o simulacích útoku na útoky pomocí **hesel**

  - Pokud má cílový účet povolené MFA a heslo je správné, účet se nezobrazuje jako ohrožený (druhý ověřovací faktor nebude úplný).

  - Soubor s heslem nesmí být větší než 10 MB. Na každém řádku použijte jedno heslo a za poslední heslo v seznamu zahrňte prázdný řádek.

- Důležité informace o Spear připojení **útoků phishing** :

  - Nemůžete poskytnout vlastní hodnotu **adresy URL přihlašovacího serveru phishing**.

  - Pokud příjemce používá k nahlášení zprávy jako podvodnou [zprávu,](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) může se stát, že pro zprávu nebudete dostávat upozornění (protože jde o simulovaný útok).

- Sestavy: po dokončení simulovaného útoku můžete sestavu zobrazit kliknutím na **Podrobnosti o útoku** .

- Podrobné pokyny a nové funkce v simulátoru útoku najdete v tématu [simulátor útoků na útoky v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
