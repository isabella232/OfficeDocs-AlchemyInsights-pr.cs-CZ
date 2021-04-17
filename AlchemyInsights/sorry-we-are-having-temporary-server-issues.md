---
title: Oprava aplikací Microsoft 365 Je nám líto, ale máme zprávy o dočasných problémech se serverem.
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835264"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Oprava zpráv aplikace Microsoft 365 "Omlouváme se, ale máme dočasné problémy se serverem".

Pokud se vám tato zpráva zobrazí, zkuste toto:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že neblokují přístup k internetu k aplikacím Microsoft 365. Podívejte [se na adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Přejděte na **Spustit** spustit a  >  zadejte **services.msc**. Ujistěte se, že jsou všechny spuštěné následující služby:
    - Automatické nastavení zařízení připojených k síti
    - Network List Service
    - Povědomí o umístění v síti
    - Protokol událostí systému Windows

Pokud jedna z těchto služeb není spuštěná, zkuste ji spustit. Pokud máte potíže se spuštěním služby, spusťte následující příkaz tak, že otevřete příkazový řádek se zvýšenými oprávněními:

**sfc /scannow**

Po dokončení tohoto příkazu restartujte počítač.

Podrobné informace najdete v tématu [Omlouváme se, ale nemůžeme se připojit k vašemu účtu. Zkuste to prosím znovu později" při aktivaci](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).