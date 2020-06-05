---
title: Problémy s přihlášením k aplikacím Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579894"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdná přihlašovací obrazovka v aplikacích Microsoft 365

Chcete-li tento problém vyřešit, vyzkoušejte následující postup:
- Nainstalujte nejnovější aktualizace pro [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Obnovení možností aplikace Internet Explorer: Přejděte na **Nástroje**  >  **k**  >  **Advanced**  >  **rozšířenému obnovení nastavení aplikace Internet Explorer** (nezapomeňte, že ztratíte vlastní nastavení), a zkuste se znovu přihlásit k Office.
- Zakažte ochranu aplikací programu Windows Defender (WDAG) nebo podobný firewall nebo antivirový program:
    1. V Ovládacích panelech přejděte na **Programy**a pak zvolte **Zapnout nebo vypnout funkce systému Windows**.
    2. Pokud je zapnutý program Ochrana aplikací programu Windows Defender, zkuste jej zakázat.<br/>
    **Poznámka:** Pravděpodobně bude nutné restartovat počítač.
- Ujistěte se, že modul plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) není blokován žádnou aplikací nebo bránou firewall/antivirovým programem.
- [Vymazání přihlašovacích údajů Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocí Správce pověření systému Windows<br/>
    **Poznámka:** Cesty registru pro Office 2016 se změnily na 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Další informace najdete [v tématu Problémy s připojením při přihlášení po aktualizaci na sestavení Office 2016 16.0.7967 ve Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).