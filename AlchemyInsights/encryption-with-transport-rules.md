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
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813861"
---
# <a name="encryption-with-transport-rules"></a>Šifrování pomocí pravidel přenosu

V [Centru pro správu Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) můžete v pravidlech toku pošty používat funkce šifrování zpráv Office (OME) ke spouštění šifrování zpráv. U podmínky Pravidlo přenosu vyberte možnost **Použít šifrování zpráv Office 365 a ochranu práv**.

- Další informace najdete v článku [Definování pravidla toku pošty pro šifrování](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- V PowerShellu použijte rutinu [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) a nastavte parametr *ApplyOME* na $true.
