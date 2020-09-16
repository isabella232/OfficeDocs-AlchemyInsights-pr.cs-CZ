---
title: Nastavení zásad schůzky
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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794327"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa zásad schůzky v Microsoft Teams

**Poznámka: změny zásad se projeví až až za 24 hodin.** Je možné, že nebudete moct okamžitě měnit nově vytvořené zásady. Počkejte 4 hodiny a zkuste znovu změnit nově vytvořenou zásadu.

Zásady schůzky se používají k řízení funkcí, které jsou k dispozici účastníkům schůzky, které jsou naplánované uživateli ve vaší organizaci. Některé funkce zásad schůzky se zatím neaktivují v centru pro správu týmů (v dokumentaci jsou označené jako nadcházející). V tomto případě nebo pokud se vám zobrazí chybová zpráva "Nemůžeme tuto zásadu aktualizovat, ale zkuste to později" v centru pro správu Microsoft Teams doporučujeme použít PowerShell k vytvoření nebo úpravě zásad schůzky v Teams. 

Další informace o zásadách schůzky najdete v následujících zdrojích:

- Informace o vytváření zásad, provádění změn a přiřazování uživatelů k zásadám najdete v tématu [Správa zásad schůzky v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Informace o změnách zásad pomocí rutin PowerShellu najdete v tématu [Team PowerShell – přehled](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Potřebujete použít [modul PowerShell Skypu pro firmy](https://www.microsoft.com/download/details.aspx?id=39366) pro zásady schůzky v Teams. 
    - Další informace najdete v [dokumentaci rutin *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

