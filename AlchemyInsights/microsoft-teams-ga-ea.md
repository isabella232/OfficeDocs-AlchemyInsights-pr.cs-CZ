---
title: Microsoft Teams – přístup hostů
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: ee38dcb5f40ea16cea1b84b9b16e86b0f52f2d89
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/13/2020
ms.locfileid: "48452221"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams – přístup hostů

Pokud potřebujete pomoct komunikovat s uživateli mimo vaši organizaci v aplikaci teams, musíte se rozhodnout, jestli chcete použít [přístup hostů nebo externí přístup (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), nebo můžete použít obojí.

Podívejte se, jaké jsou [rozdíly mezi](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) funkcemi dostupnými pro jednotlivé.  Například externí přístup (Federation) umožňuje komunikaci 1:1, jako je chat a přítomnost.  Federované uživatele se ale nemohou zúčastnit spolupráce v týmu.  Pokud chcete, aby se externí uživatel mohl připojit ke konverzacím kanálu nebo sdílet soubory, musíte zapnout přístup hostů.

**Možnost 1: zapnutí přístupu hostů** V centru pro správu týmů přejděte na [Nastavení organizace > přístup hostů](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) a zapněte možnost povolit přístup hostů do týmů.  U tenanta s ostatními výchozími nastaveními by to mělo být.  Chcete-li přizpůsobit konfiguraci přístupu pro hosty, postupujte podle pokynů v části [Kontrolní seznam pro přístup hostů](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Po dokončení musíte [počkat až 24 hodin, než](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) se nastavení projeví.

Pokud jste si jistí, že jste dokončili všechny kroky v kontrolním seznamu, a je to víc než 24 hodin, zkuste [do týmu přidat hosta](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Další informace, včetně videí, najdete [v tématu přístup hostů v Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Možnost 2: zapnutí externího přístupu (federace)** Pokud chcete taky zapnout externí přístup (federace), přejděte v centru pro správu týmů na nastavení pro celou organizaci [> externí přístup](https://admin.teams.microsoft.com/company-wide-settings/external-communications) a zapněte možnost Uživatelé mohou komunikovat s uživateli Skypu pro firmy a týmy a pak postupujte podle všech kroků, které [uživatelům týmů umožní chatovat a komunikovat s uživateli v jiné organizaci](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).
