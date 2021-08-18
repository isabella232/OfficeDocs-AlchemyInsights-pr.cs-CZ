---
title: Přenos e-mailů přes Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324355"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Nastavení multifunkčního zařízení nebo aplikace na posílání e-mailů

Informace o možnostech a postup najdete v článku [Jak nastavit multifunkční zařízení nebo aplikaci na posílání e-mailů pomocí Microsoftu 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Pokud máte zařízení nebo aplikaci, které nedávno přestaly fungovat, nejčastějšími problémy jsou:

- **Chyby související s ověřováním při odesílání klienta SMTP Auth** Nedávno jsme udělali některé změny týkající se toho, jak funguje ověřování SMTP. Další informace o řešení problémů najdete v části o neúspěšném ověřování v článku Řešení problémů s tiskárnami, skenery a [aplikacemi LOB,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)které odesílaly e-maily pomocí Microsoft 365 nebo Office 365 .
- Při zabezpečeném připojení k internetu přijímáme jenom verzi **TLS 1.2 Office 365** Pokud používáte zabezpečené připojení (TLS), ujistěte se, že vaše aplikační zařízení podporuje TLS 1.2. Další informace najdete v tématu [Příprava na TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)v Office 365 a Office 365 GCC .
 
Další problémy a řešení najdete v článku Řešení problémů s [tiskárnami, skenery](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)a lob aplikacemi, které odesílaly e-maily Microsoft 365 nebo Office 365 .

Pokud se chcete podívat na zařízení, kterých se to týká, přejděte na [Zprávu o ověření klientů SMTP](https://protection.office.com/mailflow/dashboard).

**Poznámka:** Exchange Online nepodporuje scénáře hromadné korespondence. Pokud chcete posílat hromadné komerční e-maily (například bulletiny zákazníků), měli byste použít poskytovatele třetích stran, kteří se na tyto služby specializují.
