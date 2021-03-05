---
title: Zřizování uživatelů
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481098"
---
# <a name="user-provisioning"></a>Zřizování uživatelů

- Funkce zřizování [na vyžádání umožňuje](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) zřídit uživatele a získat podrobné diagnostické nástroje o krocích, které podnikáte.
- Pokud chcete vyřešit problémy, se kterými se setkáte při zřizování uživatelů a skupin, podívejte se do průvodce odstraňováním [potíží, který](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)se týká žádných uživatelů.
- Pokud sledujete, že uživatelé nejsou zřízeni, podívejte se na protokoly zřizování [(verze Preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) v Azure Active Directory (AD). Hledání položek protokolu týkajících se konkrétního uživatele
- Opakovaným restartováním zřizování zachyťte všechny uživatele, kteří byli zmeškaní v předchozím cyklu zřizování.
- Uživatel nebo skupina pravděpodobně nebyly zřízeny, protože naše služba ještě nemá možnost uživatele vyhodnotit. Prohlédněte si pokyny, jak dlouho trvá zřizování a indikátor průběhu na stránce pro konfiguraci zřizování. Pokud se stabilní stav zadaný v části s dalšími podrobnostmi nachází před datem, kdy byl uživatel vytvořen, aktualizován nebo odstraněn, znamená to, že jsme uživatele ještě nevyhodnocili. V tomto scénáři je nejlepší počkat, až se dokončí zřizovací služba. Pokud bylo dosaženo stabilního stavu, doporučujeme restartovat uživatelské rozhraní na portálu Azure Portal.
  - Upozorňujeme, že naše služba o změnách ve zdrojovém systému (Azure Active Directory) ví jenom u uživatele nebo skupiny. Pokud odeberete uživatele nebo skupinu přímo v aplikaci (například ServiceNow), o těchto změnách víme a v závislosti na stavu uživatele ve zdrojovém systému je nevrátíme zpět. V tomto scénáři je nejlepší vrátit změnu zpět přímo v cílové aplikaci.
- Naše služba vyhodnotila uživatele nebo skupinu a určila, že by se nemělo zřřovat:
  - Pokud jste nastavili obor pro přiřazené uživatele a skupiny, zkontrolujte, jestli má aplikace přiřazený uživatel nebo skupina.
  - Pokud má aplikace přiřazené uživatele nebo skupinu, ujistěte se, že nejsou přiřazené k výchozí roli přístupu. Tuto roli nelze použít pro zřizování.
  - Pokud jste nastavili filtr rozsahu založený na atributu, přesvědčte se, zda uživatel splňuje zadaná kritéria.
  - Pokud už uživatelé existují v cílovém systému a stav uživatele ve zdrojové a cílové shodě, nebudeme už nic dalšího dalšího provést.
- Naše služba se pokusila zřídit uživatele, ale selhala. U těchto scénářů si prohlédněte kartu řešení potíží a doporučení v protokolech zřizování:
  - Atribut, který uživatel požaduje, může v Azure Active Directory chybět nebo neodpovídá formátu, který požaduje aplikace třetí strany. Například atribut Country u uživatele může být nastavený na Usa, pokud by to měl být US.
  - Atribut je referenční atribut, který v cílové aplikaci ještě neexistuje. Referenční atribut je atribut, který odkazuje na jiný objekt, například na uživatele, který je členem skupiny. ID uživatele bude v atributu člena skupiny, ale může se zpracovávat jenom v případě, že objekt uživatele, na který odkazuje, už existuje.
