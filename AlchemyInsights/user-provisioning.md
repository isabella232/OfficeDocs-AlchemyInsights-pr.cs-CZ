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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971332"
---
# <a name="user-provisioning"></a>Zřizování uživatelů

- Pomocí funkce [zřizování na vyžádání](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) můžete zřídit uživatele a získat podrobnou diagnostiku kroků.
- Pokud chcete vyřešit problémy, se kterými se setkáte při zřizování uživatelů a skupin, podívejte se na příručku pro řešení potíží, kde nejsou [zřování žádní uživatelé.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Pokud zaznamenáte, že uživatelé nejsou zřásí, přečtěte si informace v tématu Protokoly zřizování [(preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) v Azure Active Directory (AD). Vyhledejte položky protokolu týkající se konkrétního uživatele.
- Pravidelně restartujte zřizování, abyste zachytali všechny uživatele, kteří byli zmeškaní v předchozím cyklu zřizování.
- Uživatel nebo skupina možná nebyla zřízena, protože naše služba ještě neměla možnost uživatele vyhodnotit. Zkontrolujte pokyny, jak dlouho trvá zřizování, a také indikátor průběhu na stránce konfigurace zřizování. Pokud je rovnovážný stav zadaný v části Další podrobnosti před datem, kdy byl uživatel vytvořen/aktualizován/odstraněn, znamená to, že jsme uživatele zatím nevyhodnotili. V tomto scénáři je nejlepší počkat, až se služba zřizování dokončí. Pokud bylo dosaženo stabilního stavu, doporučujeme provést restartování uživatelského rozhraní na portálu Azure Portal.
  - Upozorňujeme, že naše služba ví jenom o změnách uživatele nebo skupiny ve zdrojovém systému (Azure Active Directory). Pokud je uživatel nebo skupina odebrán přímo v aplikaci (například ServiceNow), o těchto změnách nevíme a nevrátíme ho zpět na základě stavu uživatele ve zdrojovém systému. V tomto scénáři je nejlepší vrátit změnu zpět přímo v cílové aplikaci.
- Naše služba vyhodnotila uživatele nebo skupinu a určila, že by neměla být zřízena:
  - Pokud jste nastavili obor na přiřazené uživatele a skupiny, zkontrolujte, jestli je uživatel nebo skupina přiřazená k aplikaci.
  - Pokud je uživateli nebo skupině přiřazená aplikace, ujistěte se, že nejsou přiřazeny k výchozí roli přístupu. Tuto roli nelze použít pro zřizování.
  - Pokud jste nastavili filtr oborů založený na atributech, ujistěte se, že uživatel splňuje zadaná kritéria.
  - Pokud už uživatelé existují v cílovém systému a stav uživatele ve zdrojové a cílové shodě, nebudeme nic dalšího rozvíjet.
- Naše služba se pokusila zřídit uživatele a selhala. V těchto situacích si projděte kartu řešení potíží a doporučení v protokolech zřizování:
  - Požadovaný atribut uživatele může v aplikaci Azure Active Directory nebo neodpovídá formátu požadovanému aplikací třetí strany. Například atribut Země u uživatele může být nastavený na Spojené státy, pokud by měl být americký.
  - Atribut je referenční atribut, který v cílové aplikaci ještě neexistuje. Referenční atribut je atribut, který odkazuje na jiný objekt, například na uživatele, který je členem skupiny. ID uživatele by bylo v atributu člena skupiny, ale může být zpracováno jenom v případě, že objekt uživatele, na který odkazuje, už existuje.
