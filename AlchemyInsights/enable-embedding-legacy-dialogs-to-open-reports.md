---
title: Povolení vkládání starších dialogových oken k otevření sestav
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204653"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Povolení vkládání starších dialogových oken k otevření sestav

**Příznakem**

Uživatelé nemohou otevřít sestavy. "Něco se pokazilo. Další podrobnosti naleznete v technických podrobnostech."

Tato část obsahuje přehledné informace o problému a osobě, která ho má odstranit. Na obrázku vidíte tři základní strany v transakci e-mailu Office 365 - odesílatele, Office 365 a příjemce. Červeně označená oblast je oblast, ve které je obvykle potřeba problém odstranit.

Sestavy se nedaří načíst v UCI s chybou "Popisovač formuláře je null nebo není definován." Sestavy v UCI stále vyžadují starší dialogová okna, takže systém zákazníka musí mít *povoleno povolené delegacydialogsemdding.*

**Řešení**

1. Přejděte na **kartu Nastavení >správa > nastavení systému > obecné**.

2. Možnost Povolit vkládání určitých starších dialogových oken v klientovi prohlížeče sjednoceného rozhraní na **možnost Ano**.
