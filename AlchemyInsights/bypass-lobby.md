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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059589"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Řízení nastavení předsálí a úrovně účasti v Teams

Pokud chcete všem, včetně vytáčených, externích a anonymních uživatelů povolit obejít předsálí, použijte k provedení tohoto úkolu PowerShell. Tady je příklad úpravy zásad globální schůzky pro vaši organizaci.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tato rutina momentálně vyžaduje použití Skype pro firmy PowerShellu. Pokud chcete tuto rutinu nastavit, podívejte se na správu [zásad přes PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Jakmile nastavíte zásadu, musíte ji použít pro uživatele. nebo pokud jste změnili globální zásadu, automaticky se použije pro uživatele. Pokud chcete změnit zásady, musíte počkat minimálně 4 hodiny **až 24** hodin, než se zásady projeví. 

Před provedením těchto změn si před provedením těchto změn prohlédněte dokumentaci, abyste přesně pochopili, co to umožňuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Principy Teams zásad předsálí schůzky

Tato nastavení řídí, kteří účastníci schůzky čekají v předsálí před přijetím ke schůzce, a úroveň účasti, kterou mají účastníci schůzky povolenou na schůzce. PowerShell můžete použít k aktualizaci nastavení zásad schůzky, která ještě nebyla implementovaná (označená jako "brzy") v Centru pro správu Teams schůzek. Níže najdete příklad rutiny PowerShellu, která umožňuje všem uživatelům obejít předsálí.

- [Automatické přijetí lidí](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) je zásada pro organizátory, která určuje, jestli se lidé připojují ke schůzce přímo, nebo čekat v předsálí, dokud je nepřijme ověřený uživatel.

- Povolit [anonymním](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) lidem zahájit schůzku je zásada pro organizátory, která určuje, jestli se anonymní lidé, včetně uživatelů B2B a federovaných uživatelů, mohou připojit ke schůzce uživatele bez účasti ověřeného uživatele z organizace.

- Povolit [uživatelům](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) vytáčení obejít předsálí **(už** brzy) je zásada pro organizátory, která určuje, jestli se lidé, kteří se telefonicky připojují ke schůzce přímo, nebo čekají v předsálí bez ohledu na nastavení Automaticky připustit **lidi.**

- Povolit organizátorům přepsat nastavení předsálí [(už](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **brzy)** je zásada pro organizátory, která určuje, jestli  organizátor schůzky může přepsat nastavení předsálí nastavené správcem v části Automaticky připustit lidi a Povolit uživatelům vytáčení obcházet předsálí při plánování nové schůzky. 

**Poznámka:** Úplný [přehled zásad Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) schůzek najdete v tématu Správa Microsoft Teams schůzek.
