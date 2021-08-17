---
title: Šifrování pomocí pravidel přenosu
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
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079443"
---
# <a name="encryption-with-transport-rules"></a>Šifrování pomocí pravidel přenosu

V [Centru pro správu Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) můžete v pravidlech toku pošty používat funkce šifrování zpráv Office (OME) ke spouštění šifrování zpráv. U podmínky Pravidlo přenosu vyberte možnost **Použít šifrování zpráv Office 365 a ochranu práv**.

- Další informace najdete v článku [Definování pravidla toku pošty pro šifrování](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- V PowerShellu použijte rutinu [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) a nastavte parametr *ApplyOME* na $true.
