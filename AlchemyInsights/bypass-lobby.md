---
title: Obejít předsálí
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820027"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Řízení nastavení předsálí a úrovně účasti v Teams

Pokud chcete všem, včetně vytáčených, externích a anonymních uživatelů povolit obejít předsálí, použijte k provedení tohoto úkolu PowerShell. Tady je příklad úpravy zásad globální schůzky pro vaši organizaci.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tato rutina momentálně vyžaduje použití modulu PowerShell Skypu pro firmy. Pokud chcete tuto rutinu nastavit, podívejte se na správu [zásad přes PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Jakmile nastavíte zásadu, musíte ji použít pro uživatele. nebo pokud jste změnili globální zásadu, automaticky se použije pro uživatele. Pokud chcete změnit zásady, musíte počkat minimálně 4 hodiny **až 24** hodin, než se zásady projeví. 

Před provedením těchto změn si před provedením těchto změn prohlédněte dokumentaci, abyste přesně pochopili, co to umožňuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Principy řízení zásad v předsálí schůzek v Teams

Tato nastavení řídí, kteří účastníci schůzky čekají v předsálí před přijetím ke schůzce, a úroveň účasti, kterou mají účastníci schůzky povolenou na schůzce. PowerShell můžete použít k aktualizaci nastavení zásad schůzky, která ještě nebyla implementovaná (označená jako "brzy") v Centru pro správu Teams. Níže najdete příklad rutiny PowerShellu, která umožňuje všem uživatelům obejít předsálí.

- [Automatické přijetí lidí](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) je zásada pro organizátory, která určuje, jestli se lidé připojují ke schůzce přímo, nebo čekat v předsálí, dokud je nepřijme ověřený uživatel.

- Povolit [anonymním](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) lidem zahájit schůzku je zásada pro organizátory, která určuje, jestli se anonymní lidé, včetně uživatelů B2B a federovaných uživatelů, mohou připojit ke schůzce uživatele bez účasti ověřeného uživatele z organizace.

- Povolit [uživatelům](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) vytáčení obejít předsálí **(už** brzy) je zásada pro organizátory, která určuje, jestli se lidé, kteří se telefonicky připojují ke schůzce přímo, nebo čekají v předsálí bez ohledu na nastavení Automaticky připustit **lidi.**

- Povolit organizátorům přepsat nastavení předsálí [(už](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **brzy)** je zásada pro organizátory, která určuje, jestli  organizátor schůzky může přepsat nastavení předsálí nastavené správcem v části Automaticky připustit lidi a Povolit uživatelům vytáčení obcházet předsálí při plánování nové schůzky. 

**Poznámka:** Úplný [přehled zásad schůzek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) v Microsoft Teams najdete v článku Správa zásad schůzek v Teams.
