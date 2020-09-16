---
title: Problém s aktivací – teď se nemůžeme připojit
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725976"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Oprava aplikací Microsoft 365 se nemůžete připojit hned "

Pokud se zobrazí tato zpráva, zkuste toto:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, že nejsou blokovány internetové připojení k aplikacím Microsoft 365. Viz [adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Přejděte na **Spustit**  >  **Run**a zadejte **Services. msc**. Zkontrolujte, jestli jsou všechny tyto služby běžící:
    - Automatická instalace zařízení připojeného k síti
    - Služba seznam sítě
    - Povědomí o umístění v síti
    - Protokol událostí systému Windows

Pokud není některá z těchto služeb spuštěná, zkuste ji spustit. Pokud máte problém se spuštěním služby, spusťte příkazový řádek se zvýšenými oprávněními a spusťte následující příkaz:

**sfc/scannow**

Po dokončení tohoto příkazu restartujte počítač.

Podrobné informace najdete v [části "litujeme, ale nemůžeme se připojit ke svému účtu. Při aktivaci Office ze systému Microsoft 365 zkuste to znovu později](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).