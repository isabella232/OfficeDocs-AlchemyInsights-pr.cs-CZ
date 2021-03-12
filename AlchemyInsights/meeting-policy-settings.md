---
title: Nastavení zásad schůzek
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704599"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa zásad schůzek v Microsoft Teams

**Poznámka: Než se změny zásad projeví u uživatelů, může to trvat až 24 hodin.** Je možné, že nebudete moct v nově vytvořených zásadách okamžitě dělat změny. počkejte 4 hodiny a zkuste znovu upravit nově vytvořenou zásadu.

Zásady schůzek slouží k řízení funkcí, které jsou dostupné účastníkům schůzky pro schůzky naplánované uživateli ve vaší organizaci. Některé funkce zásad schůzek ještě nemusí být implementované v Centru pro správu Teams (ty jsou v dokumentaci označené jako "brzy"). Pokud se v tomto případě nebo pokud se zobrazí chybová zpráva s informací, že zásady teď nemůžeme aktualizovat, ale později to zkusit znovu. V Centru pro správu Microsoft Teams doporučujeme k vytvoření nebo úpravám zásad schůzek v Teams použít PowerShell. 

Další informace o zásadách schůzek najdete v těchto zdrojích:

- Další informace o vytváření zásad, provádění změn a přiřazování uživatelů k zásadám najdete v tématu Správa zásad [schůzek v Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Pokud chcete udělat změny zásad pomocí rutin PowerShellu, podívejte se [na přehled Teams PowerShellu.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Pro zásady schůzek v Teams musíte použít modul [PowerShell pro Skype](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) pro firmy. 
    - Další informace [najdete v dokumentaci rutin *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

