---
title: Problém s aktivací – teď se nemůžeme připojit
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744588"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Oprava Microsoft 365 aplikace "Právě teď se nemůžeme připojit"

Poznámka: Pokud používáte starší verzi Windows (například Windows 7 SP1, Windows Server 2008 R2), použijte [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) snadnou opravu k povolení protokolu TLS 1.2 jako výchozího. Další informace najdete v článku Aktualizace a povolení [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)jako výchozích zabezpečených protokolů ve WinHTTP v Windows .

Pokud se vám tato zpráva zobrazí, zkuste toto:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že neblokují přístup k internetu Microsoft 365 aplikacím. Další informace najdete v tématu Adresy URL a [rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)společnosti Microsoft.

2. Přejděte na **Spustit**  >  **spustit a** zadejte **services.msc**. Ujistěte se, že jsou všechny spuštěné následující služby:
    - Automatické nastavení zařízení připojených k síti
    - Network List Service
    - Povědomí o umístění v síti
    - Windows Protokol událostí

Pokud jedna z těchto služeb není spuštěná, zkuste ji spustit. Pokud máte potíže se spuštěním služby, spusťte následující příkaz tak, že otevřete příkazový řádek se zvýšenými oprávněními:

**sfc /scannow**

Po dokončení tohoto příkazu restartujte počítač.

Podrobné informace najdete v tématu [Omlouváme se, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)při aktivaci Office z Microsoft 365 .