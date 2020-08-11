---
title: Doplněk Teams pro Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629435"
---
# <a name="teams-add-in-for-mac"></a>Doplněk Teams pro Mac

Pokud chcete vyřešit problém s chybějícím doplňkem Teams pro Mac, postupujte takto:

**Krok 1:** Pokud máte hybridní místní Exchange Server (2016 CU3 nebo novější), pomocí nástroje Test-HMA.ps1 potvrďte, že je hybridní moderní ověřování správně nakonfigurované. Další informace najdete v článku [ověření nastavení hybridního moderního ověřování pro Outlook pro iOS a Android](https://aka.ms/AA980zq).  

**Poznámka:** Používejte formát adresy UPN (například [username@contoso.com](mailto:username@contoso.com)), ne doména \ uživatelské_jméno. Používejte to i pro uživatele s poštovními schránkami Exchange Online.

**Krok 2:** Přejděte na **Tools**  >  **účty**nástrojů... v Outlooku pro Mac a najděte a vyberte účet. Potvrďte, že uvedené uživatelské jméno je ve formátu UPN (například [username@contoso.com](mailto:username@contoso.com)).

**Krok 3:** Ověřte, jestli je uživatel licencovaným uživatelem Microsoft Teams. Uživatel musí používat předplatné Office 365 for Mac, verzi produktu 16,24 nebo novější.