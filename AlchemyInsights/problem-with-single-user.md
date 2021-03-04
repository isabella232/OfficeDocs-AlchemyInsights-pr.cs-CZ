---
title: Problém s jedním uživatelem
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429467"
---
# <a name="problem-with-single-user"></a>Problém s jedním uživatelem

- Uživatel možná nebyl zřízen, protože služba ještě nemá možnost uživatele vyhodnotit. Prohlédněte si pokyny, jak dlouho bude zřizování a indikátor průběhu na stránce pro konfiguraci zřizování trvat. Pokud se stabilní stav zadaný v části s dalšími podrobnostmi nachází před datem, kdy byl uživatel vytvořen, aktualizován nebo odstraněn, znamená to, že jsme uživatele ještě nevyhodnocili. V tomto scénáři je nejlepší počkat, až se dokončí zřizovací služba.

  - Mějte na paměti, že naše služba je o změnách uživatele ve zdrojovém systému (cloudové personální oddělení). Aby azure AD detekuje změnu a přetékal do Active Directory, musí být ve zdrojovém systému platná změna.
- Služba zřizování vyhodnocela uživatele a určila, že nemá být zřízena:
  - Pokud jste nastavili filtr rozsahu založený na atributu, přesvědčte se, zda uživatel splňuje zadaná kritéria.
  - Pokud už uživatelé existují v cílovém systému a stav uživatele ve zdrojové a cílové shodě, nebudeme už nic dalšího provést.
- Služba zřizování se pokusila zřídit uživatele, ale selhala. U těchto scénářů si prohlédněte kartu řešení potíží a doporučení v protokolech zřizování:
  - Atribut, který uživatel požaduje, může chybět v místní službě Active Directory nebo Azure AD. Například pravidla generace userPrincipalName nebo sAMAccountName negenerují správnou hodnotu.
  - Odpovídající atribut (obvykle employeeId) se nevyřešuje jedinečnému uživateli v místní službě Active Directory nebo Azure AD. Například dva uživatelé se stejným id zaměstnance ve službě AD a služba vrátí kód chyby, který označuje duplicitní cílové položky pro stejnou zdrojovou položku.

Pokud chcete zkontrolovat protokoly pro jednotlivé uživatele a skupiny, podívejte se na téma Kontrola protokolů zřizování pro problém [s konkrétním uživatelem.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
