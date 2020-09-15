---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695280"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdná přihlašovací obrazovka v aplikacích Microsoft 365

Tento problém můžete vyřešit takto:
- Nainstalujte si nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Obnovení možností Internet Exploreru: přejděte na **nástroje**  >  **Možnosti Internetu**–  >  **Rozšířené**  >  **Obnovení nastavení Internet Exploreru** (Všimněte si, že ztratíte vlastní nastavení) a zkuste se znovu přihlásit k Office.
- Zakažte ochranu Application Guard v programu Windows Defender (WDAG) nebo podobný program brány firewall nebo antivirového programu:
    1. V Ovládacích panelech přejděte na **programy**a pak zvolte **zapnout nebo vypnout funkce systému Windows**.
    2. Pokud je zapnutá ochrana Application Guard v programu Windows Defender, zkuste ho zakázat.<br/>
    **Poznámka:** Možná bude potřeba restartovat počítač.
- Ujistěte se, že [modul plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. aad. BrokerPlugin AAD není blokován žádnou aplikací ani bránou firewall/antivirový program.
- Pomocí Správce přihlašovacích údajů systému Windows [vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16,0. (Např.: \Software\Microsoft\Office\16.0\Common\Identity\)

Další informace najdete v článku [problémy s připojením při přihlášení po aktualizaci na Office 2016 Build 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).