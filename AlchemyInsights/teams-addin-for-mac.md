---
title: Teams pro Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582063"
---
# <a name="teams-add-in-for-mac"></a>Teams pro Mac

Pokud chcete vyřešit Teams pro uživatele operačního systému Mac, postupujte takto:

**Krok 1:** Pokud máte místní hybridní Exchange (2016 CU3 nebo novější), ověřte pomocí nástroje Test-HMA.ps1, že je hybridní moderní ověřování správně nakonfigurované. Další informace najdete v tématu Ověření nastavení hybridního moderního ověřování pro [Outlook pro iOS](https://aka.ms/TestHMAEAS)a Android.  

**Poznámka:** Použijte formát adresy hlavní název uživatele (například [username@contoso.com](mailto:username@contoso.com)), ne doménu\uživatelské_jméno. To můžete udělat i pro uživatele s Exchange Online poštovními schránkami.

**Krok 2:** Have the user go to **Tools**  >  **Accounts**... v Outlook pro Mac a vyhledejte a vyberte účet. Potvrďte, že uvedené uživatelské jméno je ve formátu hlavní název uživatele (například [username@contoso.com).](mailto:username@contoso.com)

**Krok 3:** Potvrďte, že uživatel je licencovaný Microsoft Teams uživatele. Uživatel musí používat předplatné Office 365 for Mac, produkt verze 16.24 nebo novější.