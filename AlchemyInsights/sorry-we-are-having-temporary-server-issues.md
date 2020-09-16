---
title: Oprava aplikací Microsoft 365 Litujeme, máme zprávu o dočasném problému se serverem.
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758238"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Oprava aplikací Microsoft 365 "litujeme, máme zprávu o dočasných problémech se serverem."

Pokud se zobrazí tato zpráva, zkuste toto:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že nejsou blokovány internetové připojení k aplikacím Microsoft 365. Podívejte [se na adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Přejděte na **Spustit**  >  **Run**a zadejte **Services. msc**. Zkontrolujte, jestli jsou všechny tyto služby běžící:
    - Automatická instalace zařízení připojeného k síti
    - Služba seznam sítě
    - Povědomí o umístění v síti
    - Protokol událostí systému Windows

Pokud není některá z těchto služeb spuštěná, zkuste ji spustit. Pokud máte problém se spuštěním služby, spusťte příkazový řádek se zvýšenými oprávněními a spusťte následující příkaz:

**sfc/scannow**

Po dokončení tohoto příkazu restartujte počítač.

Podrobné informace najdete v [části "litujeme, ale nemůžeme se připojit ke svému účtu. Při aktivaci zkuste to znovu později](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).