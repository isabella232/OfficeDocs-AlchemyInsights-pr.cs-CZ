---
title: Pokročilé koncepty ověřování platné pro Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398548"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Pokročilé koncepty ověřování platné pro Microsoft Edge

Tady jsou pokročilé koncepty ověřování, které se vztahují na Microsoft Edge:

**Proaktivní ověřování**

Když povolíte zásadu [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge se pokusí proaktivně ověřovat přihlášené uživatele prostřednictvím služeb Microsoftu. V pravidelných intervalech bude používat online službu ke kontrole aktualizovaného manifestu, který obsahuje konfiguraci, která řídí proaktivní ověřování.

Výhody: Proaktivní ověřování umožňuje ověřování klíčových služeb, jako je například stránka Nové karty Office. Pokud se jako vyhledávací modul používá Bing, zlepšuje proaktivní ověřování výkon panelu Adresa a pomáhá generovat výsledky hledání přizpůsobené potřebám vaší firmy.

**Windows Hello CredUI pro ověřování NTLM**

Pokud jednotné přihlašování (SSO) není dostupné, když se web pokusí přihlásit k uživateli pomocí mechanizmu NTLM nebo Vyjednat, umožní tato funkce uživateli sdílet přihlašovací údaje operačního systému s webem a vyhovět výzvě při ověřování pomocí uživatelského rozhraní Windows Hello Cred. Tento tok přihlašování se zobrazí jenom ve Windows 10 a jenom pro uživatele, kteří nezísknou jednotné přihlašování během výzvy NTLM nebo Vyjednat.

**Automatické přihlašování pomocí uložených hesel**

Uživatelé, kteří ukládají hesla v Microsoft Edgi, mohou povolit automatické přihlašování k webům, kde mají uložené přihlašovací údaje. Uživatelé mohou tuto funkci zapnout nebo vypnout v edge://settings/passwords a můžete ji nakonfigurovat v zásadách [správce](https://go.microsoft.com/fwlink/?linkid=2134622) hesel.
