---
title: Konfigurace šifrování zpráv pro hybridní prostředí
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 59360a040fe413e92cd880b1225b9006384a823f6e8abeb7ef922949b9a874fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035215"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>Konfigurace šifrování zpráv pro hybridní prostředí

V hybridních Exchange mohou místní uživatelé odesílat zašifrované e-maily pomocí šifrování OME (Office Message Encryption) jenom v případě, že se e-maily směrují přes Exchange Online.

Pokud chcete e-maily šifrovat pomocí OME, postupujte takto:

1. K nastavení [hybridního prostředí použijte](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) Průvodce hybridní konfigurací. Pro nastavení šifrování nejsou potřeba žádné zvláštní kroky.
2. [Nastavte si pravidla toku pošty pro šifrování](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) tak, jak byste normálně měli.


