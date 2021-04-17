---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833024"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdná přihlašovací obrazovka v aplikacích Microsoft 365

Pokud chcete tento problém vyřešit, zkuste následující postup:
- Nainstalujte si nejnovější aktualizace [pro Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetovat možnosti Internet Exploreru: Přejděte na Nástroje Možnosti internetu Upřesnit resetování nastavení  >    >    >  **Internet Exploreru** (všimněte si, že přijdete o vlastní nastavení) a zkuste se přihlásit k Office znovu.
- Zakažte Ochranu aplikací v programu Windows Defender (WDAG) nebo podobný firewall nebo antivirový program:
    1. V Ovládacích panelech přejděte na **Programy** a pak zvolte **Zapnout nebo vypnout** funkce Windows.
    2. Pokud je povolená ochrana Application Guard v programu Windows Defender, zkuste ji zakázat.<br/>
    **Poznámka:** Možná budete muset restartovat počítač.
- Ujistěte se, že modul plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) není blokován žádnou aplikací nebo bránou firewall nebo antivirovým programem.
- [Vymažte přihlašovací údaje Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce přihlašovacích údajů systému Windows.<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Další informace najdete v článku Problémy s připojením při přihlašování po aktualizaci na [build 16.0.7967 Office 2016 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).