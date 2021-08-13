---
title: Teams se nespouštěl
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813343"
---
# <a name="teams-doesnt-launch"></a>Teams se nespouštěl

Pokud se pokusíte otevřít Microsoft Teams ale nikdy se neotevře, zkuste následující postup:

1. Přejděte na **%appdata%\Microsoft\Teams**.
1. Odstraňte obsah složky.
1. Restartujte počítač a zkuste ho Teams.

Možná budete muset znovu nainstalovat Teams. Přeinstalace:

1. Odinstalace Teams pomocí Ovládacích panelů.
1. Přejděte na **%appdata%\Microsoft\Teams\Application Cache**.
1. Odstraňte obsah složky.
1. Přejděte na **%appdata%\Microsoft\teams\Cache**.
1. Odstraňte obsah složky.
1. Restartujte počítač a pak stáhněte a nainstalujte Teams.

Pokud chcete spustit diagnostiku na tenantovi pro konkrétního uživatele, který se nemůže přihlásit, spusťte nové hledání pomocí klíčového slova **TeamsUserUnableToSignIn** a postupujte podle pokynů.