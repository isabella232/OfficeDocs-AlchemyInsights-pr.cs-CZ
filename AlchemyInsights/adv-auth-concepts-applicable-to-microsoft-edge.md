---
title: Rozšířené principy ověřování vztahující se na Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573329"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Rozšířené principy ověřování vztahující se na Microsoft Edge

Následují rozšířené principy ověřování, které platí pro Microsoft Edge:

**Proaktivní ověřování**

Když povolíte zásadu [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge se pokusí aktivně ověřovat přihlášené uživatele prostřednictvím služeb Microsoftu. V pravidelných intervalech se pomocí online služby vyhledá aktualizovaný manifest, který obsahuje konfiguraci aktivního ověřování.

Výhody: proaktivní ověřování umožňuje ověřování pro klíčové služby, jako je třeba stránka nové karty Office. Pokud se jako vyhledávací stroj používá Bing, proaktivní ověřování zlepšuje výkon panelu Adresa a pomáhá vytvářet výsledky hledání podle potřeb vaší firmy.

**Windows Hello pro CredUI pro ověřování NTLM**

Pokud není k dispozici jednotné přihlašování (SSO), když se web pokusí přihlásit k uživateli prostřednictvím mechanismu NTLM nebo Negotiate, umožní vám tato funkce sdílet přihlašovací údaje operačního systému s webem a splnit ověřovací výzvu pomocí přihlašovacího uživatelského rozhraní Windows Hello. Tento tok přihlašování se zobrazí jenom ve Windows 10 a jenom uživatelům, kteří nezískají jednotné přihlašování v průběhu ověřování NTLM nebo vyjednávání.

**Automatické přihlašování pomocí uložených hesel**

Uživatelé, kteří ukládají hesla v Microsoft Edge, můžou povolit automatické přihlašování k webům, kde mají uložená přihlašovací údaje. Uživatelé můžou tuto funkci zapnout nebo vypnout v edge://settings/passwords a nakonfigurovat ji v zásadách [správce hesel](https://go.microsoft.com/fwlink/?linkid=2134622) .
