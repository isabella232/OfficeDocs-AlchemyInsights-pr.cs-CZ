---
title: Poradce při potížích s SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038951"
---
# <a name="troubleshoot-sspr"></a>Poradce při potížích s SSPR

**Mám potíže s konfigurací resetování hesla**

- Pokud jste správce a hledáte, jak povolit samoobslužné resetování hesla, podívejte se na kurz povolení [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)a konfigurace resetování hesla pro vaši organizaci. Můžete také zkontrolovat licenční [požadavky](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.
    - **Jenom uživatelé cloudu** – všechny placené skladové Office 365 (O365) nebo Azure AD Basic
    - **Cloud a/nebo** místní uživatelé – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
- Další otázky k samoobslužné resetování hesla najdete v [častých otázkách.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dostávám chybovou zprávu**

V tomto článku najdete běžné chyby a jejich řešení: [Řešení potíží s resetováním samoobslužných hesel](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mám problém se zásadou resetování hesla**

- Pokud se vaše zásada resetování hesla nechová podle očekávání nebo pokud máte dotazy týkající se zásad resetování hesla, projděte si tento článek: Zásady hesel a omezení v [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Zásady resetování hesel se nevztahují na správce. Microsoft vynucuje silnou výchozí zásadu resetování hesla dvou bran pro libovolnou roli správce Azure. Ujistěte se, že testujete u uživatele, který není správcem. Další informace o zásadách obnovení továrního nastavení správce najdete v tomto článku: [Rozdíly v zásadách obnovení správcem](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Nechci, aby moji uživatelé registroval další bezpečnostní údaje pro resetování hesla**

Data (atributy e-mailu a telefonu) pro uživatele můžete předem naplnit pomocí rozhraní API, PowerShellu nebo azure AD Připojení. Postup čtení:

- [Nasazení resetování hesla bez nutnosti registrace uživatelů](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Jaká data se používají při resetování hesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chci, aby moji uživatelé zaregistroval další bezpečnostní údaje pro resetování hesla**

1. Aby uživatelé zaregistrovali svoje bezpečnostní údaje pro samoobslužné resetování hesla tak, že je nasměrují na [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Po vyplnění dat pro uživatele (uživatelem nebo správcem) nasměrujte uživatele na aka.ms/sspr, aby mohli být vaši uživatelé oprávněni resetovat si vlastní hesla. [](https://passwordreset.microsoftonline.com/)
1. Pokud uživatelé stále mají problémy, jsou s největší pravděpodobností **federovaní** nebo synchronizovaní uživatelé **s hodnotou hash** hesel. To znamená, že se pravděpodobně jedná o problém se službou zpětného zápisu hesla.