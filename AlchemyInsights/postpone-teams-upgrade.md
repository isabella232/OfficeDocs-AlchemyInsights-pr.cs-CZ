---
title: Odložit upgrade na Teams
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741764"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Odložení upgradu týmu řízeného společností Microsoft

**Důležité**: Tento problém můžeme pomoct vyřešit pomocí diagnostické podpory, ale vypadá to, že nepoužíváte nové centrum pro správu. Pokud chcete nové centrum pro správu použít, posuňte přepínač v pravém horním rohu, který říká **nové centrum pro správu** vpravo. V novém centru pro správu klikněte na widget " **Potřebuji nápovědu?** ", zadejte "odložit upgrade týmů" a spusťte diagnostický nástroj podle pokynů.

Pokud jste obdrželi sdělení o automatizovaném upgradu založeném na Microsoftu ze Skypu pro firmy do Microsoft teams a chcete automatické upgrade odložit na pozdější datum, může se Váš globální správce přihlásit na portál pro [správu portálu](https://admin.teams.microsoft.com/dashboard) a po výběru tlačítka pro **stav aktualizace** v části Microsoft Teams upgrade vyberte tlačítko **odložit** . Pokud chcete zobrazit nové datum automatizovaného upgradu vašeho klienta na Microsoft teams, aktualizujte stránku portálu pro správu Teams.

**Poznámka:** Tlačítko **odložení** bude k dispozici pouze v případě, že jste dostali oznámení centra zpráv s cílem automatického upgradu. 

Globální správci můžou pomocí [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) získat další informace o aktuálním stavu upgradu.
