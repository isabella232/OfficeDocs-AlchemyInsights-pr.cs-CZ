---
title: Vynechat předsálí
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684943"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Řízení nastavení a úrovně účasti v Teams

Pokud chcete umožnit všem, včetně vytáčeného připojení, externích a anonymních uživatelů, **vycházet z**této věci pomocí PowerShellu. Tady je příklad změny globální zásady pro schůzku ve vaší organizaci.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Tato rutina momentálně vyžaduje použití modulu PowerShell pro firmy. Pokud chcete tuto rutinu nastavit, přečtěte si [zásady správy prostřednictvím PowerShellu](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Po nastavení zásad je potřeba ji použít pro uživatele. nebo pokud jste změnili globální zásadu, automaticky se použije pro uživatele. Pro každou změnu zásad musíte počkat alespoň **4 hodiny až 24 hodin** , aby zásady vstoupily v platnost. 

Před provedením těchto změn si přečtěte níže uvedenou dokumentaci, abyste pochopili přesně to, co umožňuje.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Principy řízení zásad v případě týmů

Tato nastavení určují, které účastníky schůzky před přijetím do schůzky čekají v předsálí, a úroveň jejich účasti, která je na schůzce povolená. Pomocí PowerShellu můžete aktualizovat nastavení zásad schůzky, která nejsou v centru pro správu Teams dosud implementovaná (označená příznakem brzy). V následujícím článku najdete příklad rutiny PowerShellu, která umožňuje všem uživatelům vynechat předsálí.

- [Automaticky připustit uživatele](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) : Jedná se o zásadu, která určuje, jestli se lidé ke schůzce můžou připojit přímo nebo počkat, dokud je nepřijmou ověřený uživatel.

- [Povolit zahájení schůzky anonymním uživatelům](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je zásada, která určuje, jestli se může anonymním lidem, včetně B2B a federovaných uživatelů, připojit ke schůzce uživatele bez ověřeného uživatele z organizace v docházkě.

- [Povolit uživatelům vytáčené komunikace obejít předsálí](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**již brzy**) je zásada pro jednotlivé organizátory, která určuje, jestli se uživatelé, kteří používají telefon, můžou připojit ke schůzce přímo nebo počkat v předsálí bez ohledu na nastavení **automaticky povolit uživatele** .

- [Povolit organizátorům přepsat nastavení](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) informací (**už brzy**) je zásada pro jednotlivé organizátory, která určuje, jestli může organizátor schůzky přepsat nastavení s informacemi, které správce nastavil **automaticky** a **povolí uživatelům vytáčeného připojení, aby** při plánování nové schůzky tento předsálí vycházel.

**Poznámka:** Přečtěte si téma [Správa zásad schůzky v Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , kde najdete kompletní přehled zásad schůzky v Microsoft Teams.
