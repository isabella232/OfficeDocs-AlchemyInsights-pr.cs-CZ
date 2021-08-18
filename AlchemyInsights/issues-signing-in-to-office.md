---
title: Problémy s přihlášením k Microsoft 365 aplikacím
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088029"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdná přihlašovací obrazovka v Microsoft 365 aplikacích

Pokud chcete tento problém vyřešit, zkuste následující postup:
- Nainstalujte si nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [a Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetovat možnosti Internet Exploreru: Přejděte na Nástroje Možnosti internetu Upřesnit obnovení internet  >    >    >  **exploreru Nastavení** (všimněte si, že přijdete o vlastní nastavení) a zkuste se přihlásit k Office znovu.
- Zakažte Ochrana Application Guard v programu Windows Defender (WDAG) nebo podobný firewall nebo antivirový program:
    1. V Ovládacích panelech přejděte **na** Programy a pak zvolte **Zapnout Windows nebo vypnout**.
    2. Pokud Ochrana Application Guard v programu Windows Defender povoleno, zkuste ho zakázat.<br/>
    **Poznámka:** Možná budete muset restartovat počítač.
- Ujistěte se, že modul plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) není blokován žádnou aplikací nebo bránou firewall nebo antivirovým programem.
- [Vymažte Office přihlašovací údaje](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows Správce přihlašovacích údajů.<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Další informace najdete v článku Problémy s připojením při přihlašování po aktualizaci na [Office 2016 build 16.0.7967 v Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).