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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039959"
---
# <a name="problems-resetting-password"></a>Problémy s resetováním hesla

Tady jsou některé problémy, se které vám můžou při resetování hesla a možných řešeních čelit:

**Mám problém s resetováním hesla, který není zahrnutý v jiných kategoriích.**

- Ujistěte se, že máte oprávnění k resetování hesel. Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů. Globální správci můžou resetovat hesla dalších privilegovaných správců.
- Ujistěte se, že rozumíte licenčním požadavkům:
    - Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.
        - Jenom uživatelé cloudu – všechny Office 365 SKU (O365) nebo Azure AD Basic
        - Cloud a/nebo místní uživatelé – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
        - Další informace o licenčních požadavcích najdete v článku Licenční požadavky pro samoobslužné resetování [hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mám problémy s testováním nastavené zásady resetování hesla**

- Replikace zásad v poslední době může trvat několik minut ve všech datových centrech a koncových bodech. Fyzická vzdálenost od datového centra bude mít vliv také na to, jak rychle se změny použijí.
- Testujte s koncovým uživatelem, ne správcem a pilotním projektem s malou sadu uživatelů. Zásady nakonfigurované na portálu Azure Portal platí jenom pro koncové uživatele, ne pro správce. Microsoft vynucuje silnou výchozí zásadu resetování hesla dvou bran pro libovolnou roli správce Azure (Příklad: Globální správce, Správce technické podpory, Správce hesel atd.)
    - Přečtěte si další [informace o zásadách pro správce](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Chci nasadit resetování hesla, ale nechci, aby moji uživatelé zaregistrovat další bezpečnostní údaje**

Předplácete data pro uživatele, aby to nechcete! - Jako správce můžete nastavit vlastnosti telefonu a e-mailu pro uživatele před tím, než ve vaší organizaci začnete resetovat heslo. Můžete to udělat pomocí rozhraní API, PowerShellu nebo Azure AD Připojení. Další informace najdete tady:
- [Nasazení resetování hesla bez nutnosti registrace uživatelů](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Jaká data se používají při resetování hesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tlačítko pro resetování hesla je šedé**

Nejste oprávněni resetovat hesla tohoto uživatele. Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů. Globální správci můžou resetovat hesla dalších privilegovaných správců.

**Nevidím okno pro resetování hesla**

K resetování hesel nejste oprávněni. Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů. Globální správci můžou resetovat hesla dalších privilegovaných správců.

**V resetování hesla nevidím okno místní integrace**

- Okno místní integrace se zobrazuje jenom v hybridních prostředích, což znamená, že k manipulaci s hesly místního uživatele používáte zpětný zápis hesla.
- Tento list se zobrazí, pokud:
    - Nepou3/4ít zpětný zápis hesla
    - Došlo k problému s instalací nebo připojením zpětného zápisu hesla.
    - Došlo k problému s instalací nebo připojením služby Azure AD Připojení
    - Další kroky pro řešení problémů s zpětným zápisem hesla najdete v části Poradce při potížích s zpětným [zápisem hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nevím, jak resetovat heslo uživatele**

1. Přihlaste se k portálu Azure portal jako příslušný správce.
1. Přejděte do okna Uživatelé a skupiny a vyberte **Všichni uživatelé**.
1. V seznamu vyberte uživatele.
1. U vybraného uživatele vyberte Přehled **a** potom na panelu příkazů klikněte na **Resetovat heslo.**
1. Postupujte podle pokynů na obrazovce.
    - Resetuje se jenom prostřednictvím zpětného zápisu hesla pro podporu portálu Azure Portal.

**Resetování hesla místního uživatele z portálu Office 365 Admin nebo mobilní aplikace Office 365 ale uživatel se pořád nemůže přihlásit**

Zpětný zápis hesla není na tomto portálu podporovaný. Resetování hesla uživatele znovu na portálu Azure Portal – portal.azure.com

