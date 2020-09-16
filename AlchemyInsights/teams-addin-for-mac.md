---
title: Doplněk Teams pro Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670321"
---
# <a name="teams-add-in-for-mac"></a>Doplněk Teams pro Mac

Pokud chcete vyřešit problém s chybějícím doplňkem Teams pro Mac, postupujte takto:

**Krok 1:** Pokud máte hybridní místní Exchange Server (2016 CU3 nebo novější), pomocí nástroje Test-HMA.ps1 potvrďte, že je hybridní moderní ověřování správně nakonfigurované. Další informace najdete v článku [ověření nastavení hybridního moderního ověřování pro Outlook pro iOS a Android](https://aka.ms/AA980zq).  

**Poznámka:** Používejte formát adresy UPN (například [username@contoso.com](mailto:username@contoso.com)), ne doména \ uživatelské_jméno. Používejte to i pro uživatele s poštovními schránkami Exchange Online.

**Krok 2:** Přejděte na **Tools**  >  **účty**nástrojů... v Outlooku pro Mac a najděte a vyberte účet. Potvrďte, že uvedené uživatelské jméno je ve formátu UPN (například [username@contoso.com](mailto:username@contoso.com)).

**Krok 3:** Ověřte, jestli je uživatel licencovaným uživatelem Microsoft Teams. Uživatel musí používat předplatné Office 365 for Mac, verzi produktu 16,24 nebo novější.