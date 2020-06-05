---
title: Oprava aplikací Microsoft 365 Omlouváme se, máme zprávu o dočasných problémech se serverem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582696"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Oprava zprávy Aplikace Microsoft 365 "Omlouváme se, máme problémy s dočasným serverem"

Pokud se zobrazí tato zpráva, vyzkoušejte následující postup:

1. Zkontrolujte nastavení brány firewall, antivirového softwaru a proxy serveru a ověřte, zda neblokují přístup k Internetu aplikacím Microsoft 365. Viz [adresy URL a rozsahy IP adres](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Přejděte na **spustit**  >  **Run**a zadejte **soubor services.msc**. Ujistěte se, že jsou spuštěny všechny následující služby:
    - Automatické nastavení síťových připojených zařízení
    - Služba seznamu sítí
    - Povědomí o poloze v síti
    - Protokol událostí systému Windows

Pokud není spuštěna jedna z těchto služeb, zkuste ji spustit. Pokud máte potíže se spuštěním služby, spusťte následující příkaz otevřením příkazového řádku se zvýšenými oprávněními:

**sfc /scannow**

Po dokončení tohoto příkazu restartujte počítač.

Podrobné informace naleznete v [tématu "Omlouváme se, ale nemůžeme se připojit k vašemu účtu. Opakujte akci později" při aktivaci](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).