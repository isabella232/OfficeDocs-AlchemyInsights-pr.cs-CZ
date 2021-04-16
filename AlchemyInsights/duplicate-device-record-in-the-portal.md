---
title: Duplicitní záznam zařízení na portálu.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814509"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplicitní záznam zařízení na portálu.

Pokud zařízení nehlásí správný přehled o stavu na stránce Správce konfigurace, můžou se vám na portálu zobrazovat dva záznamy.  Pokud chcete zkontrolovat stav konkrétního zařízení, podívejte se do sloupce **Spoluspravované** na zařízení v konzole Správce konfigurace. Pokud není sloupec zobrazený, můžete ho přidat kliknutím pravým tlačítkem myši na záhlaví sloupce a vybrat ho ze seznamu.

Spoluspravovaná hodnota musí být **Ano**. Pokud je hodnota **Ne**, otevřete na klientském zařízení aplet Správce konfigurace a zkontrolujte **vlastnosti spolusprávy** na kartě Obecné.

- Pokud je hodnota **Povolena**, znamená to, že se jedná o problémy komunikace klienta s bodem správy. Abyste mohli prozkoumat potenciální problémy s připojením, podívejte se prosím na **CcmMessaging. log** na zařízení.

- Pokud je hodnota **Zakázaná** a zařízení se registruje v Intune, ujistěte se prosím, že zařízení dostalo zásadu pro spolusprávu, a to tak, že na zařízení zkontrolujete **CoManagementHandler.log.**
