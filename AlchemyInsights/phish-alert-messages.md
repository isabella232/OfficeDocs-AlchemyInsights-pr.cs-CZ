---
title: 2491 Upozornění na e-mailové zprávy z zásady Phish Delivered due to tenant or user override
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316351"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozornění na e-mailové zprávy z zásady Phish Delivered due to tenant or user override

Výchozí zásada upozornění s názvem **Phish Delivered z** důvodu přepsání tenanta nebo uživatele je dostupná v organizacích s microsoft defenderem pro licence Office 365 P1 a P2. Pokud jste dostali toto upozornění, tady je postup, jak prozkoumat:

1. Ve zprávě s upozorněním klikněte **na Zobrazit upozornění** a přejděte na stránku Upozornění na Microsoft 365 Defender portálu. 

2. Výběrem upozornění zobrazíte možnost Zobrazit **seznam zpráv** nebo Zobrazit zprávy **v Průzkumníkovi.** Obě tyto možnosti vás zavezou k podrobnostem zprávy, která obsahuje ID zprávy. Všimněte si, že odkaz Průzkumníka hrozeb automaticky vyfiltruje zprávy, které splňují kritéria upozornění. Možná budete muset upravit filtr data v Průzkumníkovi hrozeb.

Zpráva útoku phishing byla doručena z důvodu ručně nakonfigurovaného přepsání:

- Povolený odesílatel nebo doména nastavená uživatelem
- Povolený odesílatel nebo doména nastavená správcem v zásadách ochrany proti spamu
- Povolená IP adresa v zásadách filtru připojení
- Pravidlo toku pošty (označované taky jako pravidlo přenosu), které je nakonfigurované tak, aby povoloval zprávy.

Pokud se domníváte, že zpráva [](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) byla nesprávně označená jako phishing, nahlásit zprávu Microsoftu pomocí odeslání správcem.

Uživatelé mohou pomocí doplňku Zpráva [sestavy](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) nebo Nahlásit phishing v aplikaci Outlook odesílat ukázky zpráv do Microsoftu.
