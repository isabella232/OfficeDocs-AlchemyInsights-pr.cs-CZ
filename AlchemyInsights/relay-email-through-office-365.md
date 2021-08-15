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
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024199"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Nastavení multifunkčního zařízení nebo aplikace na posílání e-mailů

Informace o možnostech a postup najdete v článku [Jak nastavit multifunkční zařízení nebo aplikaci na posílání e-mailů pomocí Microsoftu 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Pokud máte zařízení nebo aplikaci, které nedávno přestaly fungovat, nejčastějšími problémy jsou:

- **Chyby související s ověřováním při odesílání klienta SMTP Auth** Nedávno jsme udělali některé změny týkající se toho, jak funguje ověřování SMTP. Další informace o řešení problémů najdete v části o neúspěšném ověřování v článku Řešení problémů s tiskárnami, skenery a [aplikacemi LOB,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)které odesílaly e-maily pomocí Microsoft 365 nebo Office 365 .
- Při vytváření zabezpečeného připojení k síti přijímáme jenom verzi **TLS 1.2 Office 365** Pokud používáte zabezpečené připojení (TLS), ujistěte se, že vaše aplikační zařízení podporuje TLS 1.2. Další informace najdete v tématu [Příprava na TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)v Office 365 a Office 365 GCC .
 
Další problémy a řešení najdete v článku Řešení problémů s tiskárnami, skenery a lob aplikacemi, které odesílaly e-maily [Microsoft 365 nebo Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Pokud se chcete podívat na zařízení, kterých se to týká, přejděte na [Zprávu o ověření klientů SMTP](https://protection.office.com/mailflow/dashboard).

**Poznámka:** Exchange Online scénáře hromadné korespondence. Pokud chcete posílat hromadné komerční e-maily (například bulletiny zákazníků), měli byste použít poskytovatele třetích stran, kteří se specializují na tyto služby.
