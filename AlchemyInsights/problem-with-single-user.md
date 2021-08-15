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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960144"
---
# <a name="problem-with-single-user"></a>Problém s jedním uživatelem

- Uživatel možná nebyl zřízen, protože služba ještě neměla možnost uživatele vyhodnotit. Zkontrolujte pokyny, jak dlouho trvá zřizování, a také indikátor průběhu na stránce konfigurace zřizování. Pokud je rovnovážný stav zadaný v části Další podrobnosti před datem, kdy byl uživatel vytvořen/aktualizován/odstraněn, znamená to, že jsme uživatele zatím nevyhodnotili. V tomto scénáři je nejlepší počkat, až se služba zřizování dokončí.

  - Upozorňujeme, že naše služba ví jenom o změnách uživatele ve zdrojovém systému (Cloud HR). Aby Služba Azure AD detekuje změnu a přetékala do služby Active Directory, musí být ve zdrojovém systému platná změna.
- Služba zřizování uživatele vyhodnotila a určila, že by neměla být zřízena:
  - Pokud jste nastavili filtr oborů založený na atributech, ujistěte se, že uživatel splňuje zadaná kritéria.
  - Pokud už uživatelé existují v cílovém systému a stav uživatele ve zdrojové a cílové shodě, nebudeme nic dalšího rozvíjet.
- Služba zřizování se pokusila zřídit uživatele a selhala. V těchto situacích si projděte kartu řešení potíží a doporučení v protokolech zřizování:
  - V místní službě Active Directory nebo v Azure AD může chybět povinný atribut uživatele. Například pravidla generování userPrincipalName nebo sAMAccountName nevygenerují správnou hodnotu.
  - Odpovídající atribut (obvykle id_zaměstnance) se nevyřešuje jedinečnému uživateli v místní službě Active Directory nebo Azure AD. Ve službě AD jsou například dva uživatelé se stejným idm zaměstnance a služba vrátí kód chyby označující duplicitní cílové položky pro stejnou zdrojovou položku.

Pokud chcete zkontrolovat protokoly pro jednoho uživatele a skupiny, podívejte se na téma Kontrola protokolů zřizování pro problém [s konkrétním uživatelem](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
