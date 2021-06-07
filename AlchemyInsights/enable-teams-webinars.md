---
title: Povolení Teams webináře
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793582"
---
# <a name="enable-teams-webinars"></a>Povolení Teams webináře

Webináře jsou ve výchozím nastavení povolené. Pomocí příkazů PowerShellu můžete spravovat, kdo Teams plánovat a registrovat Teams Teams webináře.

- Všichni uživatelé, kteří mohou vytvořit schůzku, mohou také vytvořit webinářovou schůzku. Pokud chcete spravovat, kdo může plánovat Teams webináře, použijte *AllowMeetingRegistration*. 
- Ve výchozím nastavení *je funkce WhoCanRegister* povolená a nastavená na **Everyone (Všichni).** Pokud chcete registraci schůzky vypnout, nastavte *AllowMeetingRegistration na* **False**.

Pokud chcete tato nastavení změnit, musíte si [Teams PowerShellu](/microsoftteams/teams-powershell-install). Zásady schůzek se také vynucuje na Teams webináře. Pokud je například anonymní připojení vypnuté v nastavení schůzky, anonymní uživatelé se neschová k webináři.

Další informace o konfiguraci, kdo se může registrovat pro webináře, najdete v tématu Konfigurace, kdo se [může zaregistrovat pro webináře](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Další informace o nastavení microsoftových seznamů najdete v tématu [Nastavení řízení pro seznamy Microsoft](/sharepoint/control-lists).