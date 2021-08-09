---
title: Koncepty rozšířeného ověřování platné pro Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934358"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Koncepty rozšířeného ověřování platné pro Microsoft Edge

Následující koncepty rozšířeného ověřování platí pro Microsoft Edge:

**Proaktivní ověřování**

Když povolíte zásadu [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge se pokusí proaktivně ověřovat přihlášené uživatele prostřednictvím služby Microsoft. V pravidelných intervalech bude používat online službu ke kontrole aktualizovaného manifestu, který obsahuje konfiguraci, která řídí proaktivní ověřování.

Výhody: Proaktivní ověřování umožňuje ověřování klíčových služeb, jako je Office nová karta. Pokud se Bing jako vyhledávací modul, proaktivní ověřování zlepšuje výkon panelu adresa a pomáhá generovat výsledky hledání přizpůsobené potřebám vaší firmy.

**Windows Hello CredUI pro ověřování NTLM**

Pokud jednotné přihlašování (SSO) není k dispozici, když se web pokusí přihlásit k uživateli pomocí mechanizmu NTLM nebo Vyjednat, tato funkce uživateli umožní sdílet přihlašovací údaje operačního systému s webem a vyhovět výzvě při ověřování pomocí uživatelského rozhraní Windows Hello Cred. Tento tok přihlašování se zobrazí jenom v Windows 10 a jenom pro uživatele, kteří nezísknou jednotné přihlašování během výzvy NTLM nebo Vyjednat.

**Automatické přihlašování pomocí uložených hesel**

Uživatelé, kteří hesla ukládají do Microsoft Edge, mohou povolit automatické přihlašování k webům, na kterých mají uložené přihlašovací údaje. Uživatelé mohou tuto funkci zapnout nebo vypnout v edge://settings/passwords a můžete ji nakonfigurovat v zásadách [správce](https://go.microsoft.com/fwlink/?linkid=2134622) hesel.
