---
title: e-mailové zprávy s výstrahou 2491 z zásady "phishing dodáno" v důsledku zásad přepsání tenanta nebo uživatele
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728604"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorňovat e-mailové zprávy z "funkce phishing dodaná z důvodu zásad přepsání tenanta nebo uživatele"

Výchozí zásada upozornění s názvem "phishing Doručená z důvodu přepisu tenanta nebo uživatele" byla zahrnuta do tenanta prostřednictvím licencí Office 365 ATP. Pokud jste dostali toto upozornění, postupujte takto:

1. Kliknutím na **Zobrazit** upozornění v okně upozornění přejděte na stránku **Upozornění** v centru zabezpečení &.

2. Výběrem výstrahy zobrazíte možnost **Zobrazit seznam zpráv** nebo **Zobrazit zprávy v Průzkumníkovi**. V obou těchto možnostech se zobrazí podrobnosti zprávy, která obsahuje ID zprávy. Uvědomte si, že odkaz v Průzkumníku hrozeb automaticky filtruje zprávy, které splňují kritéria upozornění. Možná bude potřeba upravit filtr data v Průzkumníku hrozeb.

Zpráva útoku phishing byla doručena z důvodu ručně konfigurovaného přepsání:

- Povoleného odesílatele nebo domény nastavené uživatelem.

- Povolený odesílatel nebo doména nastavená správcem v zásadách ochrany proti nevyžádané poště.

- Povolená IP adresa v zásadách filtru připojení.

- Pravidlo toku pošty (známé taky jako pravidlo přenosu), které je nakonfigurované tak, aby umožňovalo zprávy ve službě.

Pokud se domníváte, že zpráva byla nesprávně označená jako phishing, [použijte k odeslání](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) ukázek zpráv do Microsoft.
