---
title: Duplicitní záznam zařízení na portálu.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678497"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplicitní záznam zařízení na portálu.

Pokud zařízení nehlásí správný přehled o stavu na stránce Správce konfigurace, můžou se vám na portálu zobrazovat dva záznamy.  Pokud chcete zkontrolovat stav konkrétního zařízení, podívejte se do sloupce **Spoluspravované** na zařízení v konzole Správce konfigurace. Pokud není sloupec zobrazený, můžete ho přidat kliknutím pravým tlačítkem myši na záhlaví sloupce a vybrat ho ze seznamu.

Spoluspravovaná hodnota musí být **Ano**. Pokud je hodnota**Ne**, otevřete na klientském zařízení aplet Správce konfigurace a zkontrolujte **vlastnosti spolusprávy** na kartě Obecné.

- Pokud je hodnota**Povolena**, znamená to, že se jedná o problémy komunikace klienta s bodem správy. Abyste mohli prozkoumat potenciální problémy s připojením, podívejte se prosím na **CcmMessaging. log** na zařízení.

- Pokud je hodnota **Zakázaná** a zařízení se registruje v Intune, ujistěte se prosím, že zařízení dostalo zásadu pro spolusprávu, a to tak, že na zařízení zkontrolujete **CoManagementHandler.log. **
