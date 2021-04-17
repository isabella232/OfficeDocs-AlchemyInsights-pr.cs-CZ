---
title: Nastavení zásad schůzky
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825436"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa zásad schůzek v Microsoft Teams

**Poznámka: Může trvat až 24 hodin, než se změny zásad projeví pro uživatele.** V nově vytvořených zásadách možná nebudete moct okamžitě dělat změny. počkejte 4 hodiny a zkuste znovu upravit nově vytvořenou zásadu.

Zásady schůzek slouží k řízení funkcí, které jsou dostupné účastníkům schůzky pro schůzky naplánované uživateli ve vaší organizaci. Některé funkce zásad schůzek ještě nemusí být implementované v Centru pro správu Teams (ty jsou v dokumentaci označené jako "brzy"). V tomto případě nebo pokud se vám v Centru pro správu Microsoft Teams zobrazí chybová zpráva, třeba "Zásady teď nemůžeme aktualizovat, ale zkuste to znovu později", doporučujeme k vytvoření nebo úpravě zásad schůzek v Teams použít PowerShell. 

Další informace o zásadách schůzek najdete v těchto zdrojích:

- Další informace o vytváření zásad, provádění změn a přiřazování uživatelů k zásadám najdete v tématu Správa zásad [schůzek v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pokud chcete provádět změny zásad pomocí rutin PowerShellu, podívejte se na [přehled Teams PowerShellu.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Pro zásady schůzek v Teams musíte použít modul [PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Skypu pro firmy. 
    - Další informace najdete v dokumentaci rutin [*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

