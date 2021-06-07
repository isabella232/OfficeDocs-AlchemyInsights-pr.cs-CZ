---
title: Správa registrace webináře
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793618"
---
# <a name="manage-webinar-registration"></a>Správa registrace webináře

Pomocí příkazů Powershellu můžete Teams, kdo se Teams webináře zaregistrovat. Informace o Teams PowerShellu najdete [v Teams PowerShellu.](/microsoftteams/teams-powershell-install) 

Ve výchozím nastavení *je funkce WhoCanRegister* povolená a nastavená na **Hodnotu EveryoneInCompany**. Pokud chcete povolit registraci všem uživatelům, včetně anonymních  uživatelů, musíte pomocí příkazu Powershellu nastavit zásady schůzky na Všichni:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Poznámka:** Pokud je anonymní připojení v nastavení schůzky vypnuté, anonymní uživatelé se neschová k webináři. Další informace a povolení tohoto nastavení najdete v tématu [Správa nastavení schůzky v Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Pokud chcete registraci schůzky vypnout, nastavte *AllowMeetingRegistration na* **False**.

Další informace o konfiguraci, kdo se může registrovat pro webináře, najdete v tématu Konfigurace, kdo se [může zaregistrovat pro webináře](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Další informace o nastavení microsoftových seznamů najdete v tématu [Nastavení řízení pro seznamy Microsoft](/sharepoint/control-lists).
