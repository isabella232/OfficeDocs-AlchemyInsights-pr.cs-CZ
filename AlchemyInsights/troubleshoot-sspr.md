---
title: Řešení potíží s SSPR
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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429472"
---
# <a name="troubleshoot-sspr"></a>Řešení potíží s SSPR

**Mám problémy s konfigurací resetování hesla**

- Pokud jste správce a hledáte, jak povolit samoobslužné resetování hesla, podívejte se, jak v organizaci nakonfigurovat resetování hesla pomocí funkce Kurz povolte nástroj [SSPR.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr) Možná si taky budete chtít prohlédněte licenční [požadavky.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.
    - **Jenom cloudové uživatele** – všechny placené SKU Office 365 (O365) nebo Azure AD Basic
    - **Cloudové a místní** uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
- Další informace o samoobslužných resetování hesel najdete v [častých otázkách.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zobrazí se mi chybová zpráva**

V tomto článku najdete informace o běžných chybách a jejich řešeních: [Řešení samoobslužných resetování hesel](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mám problém se zásadou pro resetování hesla**

- Pokud se vaše zásada resetování hesla nechová podle očekávání nebo máte dotazy k zásadám resetování hesla, projděte si tento článek: Zásady hesel a omezení v [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Zásady pro resetování hesel se nevztahují na správce. Microsoft vynucuje silné výchozí zásady resetování hesla ve dvou bránách pro libovolnou roli správce Azure. Ujistěte se, že testujete s uživatelem, který není správcem. Další informace o resetování zásad správce najdete v tomto článku: Rozdíly [v zásadách resetování správcem.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nechci, aby uživatelé zaregistroval další bezpečnostní údaje pro resetování hesla.**

Data (atributy e-mailu a telefonu) pro uživatele můžete předem vyplnit pomocí rozhraní API, PowerShellu nebo Azure AD Connect. Jak na to:

- [Nasazení resetování hesla bez nutnosti registrace uživatelů](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Jaká data se používají při resetování hesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chci, aby si uživatelé zaregistroval(a) další bezpečnostní údaje pro resetování hesla.**

1. Vemte uživatele, aby si zaregistrovali svoje bezpečnostní údaje k samoobslužnému resetování hesla tak, že je nasměrujete [na aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Po naplnění dat uživatelem (uživatelem nebo správcem) nasměrujte [](https://passwordreset.microsoftonline.com/) uživatele na správce, aby aka.ms/sspr aby mohli uživatelé obnovovat svá vlastní hesla.
1. Pokud se u uživatelů pořád dochází k problémům, jsou s největší pravděpodobností **federovaní** nebo synchronizovaní uživatelé **s hodnotou hash** hesel. To znamená, že může být nějaký problém se službou zpětného zápisu hesel.