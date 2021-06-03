---
title: Endpoint DLP not deployed to user's device
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731321"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Endpoint DLP not deployed to user's device

Pokud se na zařízení uživatele nepou3/4ít nastavení Ochrana před únikem dat koncového bodu, potvrďte, že splňujete tyto požadavky:

- Windows 10 zařízení je nainstalovaný build x64 1809 nebo novější.
- Klient antimalwaru verze 4.18.2009.7 nebo novější je nainstalovaný.
- Zařízení je **jedním z** těchto:
    
    - Azure Active Directory (Azure AD) připojeno
    - Hybridní připojení k Azure AD
    - Zaregistrovaná AAD

- Pokud chcete vynutit akce zásad, ujistěte se, Chromium na zařízení koncového bodu je nainstalovaný prohlížeč Microsoft Chromium Edge.

Další požadavky pro nasazení funkce DLP koncového bodu najdete v tématu Začínáme s prevencí [ztráty dat koncového bodu](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).