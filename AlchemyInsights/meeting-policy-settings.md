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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925158"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Správa zásad schůzek v Microsoft Teams

**Poznámka: Může trvat až 24 hodin, než se změny zásad projeví pro uživatele.** V nově vytvořených zásadách možná nebudete moct okamžitě dělat změny. počkejte 4 hodiny a zkuste znovu upravit nově vytvořenou zásadu.

Zásady schůzek slouží k řízení funkcí, které jsou dostupné účastníkům schůzky pro schůzky naplánované uživateli ve vaší organizaci. Některé funkce zásad schůzky nemusí být v Centru pro správu Teams ještě implementované (v dokumentaci jsou označené jako "brzy"). V tomto případě nebo pokud se vám v Centru pro správu Microsoft Teams zobrazí chybová zpráva, jako je "Zásady teď nemůžeme aktualizovat, ale zkuste to znovu později", doporučujeme k vytvoření Teams úpravám zásad schůzek použít PowerShell. 

Další informace o zásadách schůzek najdete v těchto zdrojích:

- Informace o vytváření zásad, provádění změn a přiřazování uživatelů k zásadám najdete v tématu Správa zásad schůzek v [Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Informace o změnách zásad pomocí rutin PowerShellu najdete [v Teams PowerShellu .](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Pro zásady schůzek [musíte Skype pro firmy powershellový](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) modul Teams schůzek. 
    - Další informace najdete v dokumentaci rutin [*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

