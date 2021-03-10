---
title: Problém s resetováním hesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693392"
---
# <a name="problems-resetting-password"></a>Problémy s resetováním hesla

Tady jsou některé problémy, se které se můžou zobrazit při resetování hesla, a možná řešení:

**Mám problém s resetováním hesla, který není zahrnutý v ostatních kategoriích**

- Ujistěte se, že máte oprávnění k resetování hesel. Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů. Globální správci můžou taky resetovat hesla jiných privilegovaných správců.
- Ujistěte se, že rozumíte licenčním požadavkům:
    - Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.
        - Jenom cloudové uživatele – všechny placené SKU Office 365 (O365) nebo Azure AD Basic
        - Cloudové a místní uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
        - Další informace o licenčních požadavcích najdete v článku Licenční požadavky pro samoobslužné resetování [hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mám problémy s testováním nastavené zásady resetování hesla**

- Může trvat několik minut, než se použité zásady replikují do všech datových center a koncových bodů. Na to, jak rychle se změny použijí, ovlivní taky fyzická vzdálenost od datového centra.
- Testujte s koncovým uživatelem, ne s správcem, a pilotním testováním s malou sadu uživatelů. Zásady nakonfigurované na portálu Azure Portal platí JENOM pro koncové uživatele, ne pro správce. Microsoft vynucuje silné výchozí zásady resetování hesla ve dvou bránách pro libovolnou roli správce Azure (Příklad: Globální správce, Správce helpdesku, Správce hesel atd.)
    - Přečtěte si další [informace o zásadách pro správce.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Chci nasadit resetování hesla, ale nechci, aby uživatelé zaregistroval další bezpečnostní údaje**

Data uživatelů můžete předem vyplnit, takže je nemusíte vyplnit. Jako správce můžete před zahájením resetování hesla pro vaši organizaci nastavit vlastnosti telefonu a e-mailu pro uživatele. Můžete to udělat pomocí rozhraní API, PowerShellu nebo Azure AD Connect. Další informace najdete tady:
- [Nasazení resetování hesla bez nutnosti registrace uživatelů](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Jaká data se používají při resetování hesla?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tlačítko pro resetování hesla se zobrazí šedě**

K resetování hesel tohoto uživatele nejste oprávněni. Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů. Globální správci můžou taky resetovat hesla jiných privilegovaných správců.

**Nevidím list pro resetování hesla**

K resetování hesel máte oprávnění. Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů. Globální správci můžou taky resetovat hesla jiných privilegovaných správců.

**Při resetování hesla nevidím místní integraci s listy**

- Místní integrace se zobrazuje jenom v hybridních prostředích, což znamená, že používáte k práci s hesly místních uživatelů zpětný zápis hesel.
- Tento list se nezekoumá, pokud:
    - Používáte bez zpětného zápisu hesla
    - Došlo k problému s instalací nebo připojením zpětného zápisu hesla
    - Došlo k problému s instalací nebo připojením služby Azure AD Connect.
    - Další kroky pro řešení problémů s zpětným zápisem hesla najdete v části Řešení potíží [se zápisem hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nevím, jak resetovat heslo uživatele**

1. Přihlaste se k portálu Azure Portal jako příslušný správce.
1. Přejděte do okna Uživatelé a skupiny a vyberte **Všichni uživatelé.**
1. Vyberte uživatele ze seznamu.
1. Pro vybraného uživatele vyberte **Přehled** a potom na panelu příkazů klikněte na **Resetovat heslo.**
1. Postupujte podle pokynů na obrazovce.
    - Obnovení pouze prostřednictvím zpětného zápisu hesla pro podporu na portálu Azure Portal

**Resetování hesla místního uživatele z portálu pro správu Office 365 nebo mobilní aplikace Office 365, ale uživatel se pořád nemůže přihlásit**

Na tomto portálu se nepodporuje zpětný zápis hesel. Resetování uživatelského hesla znovu na portálu Azure Portal – portal.azure.com

