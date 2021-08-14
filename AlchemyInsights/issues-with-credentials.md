---
title: Problémy s přihlašovacími údaji
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986812"
---
# <a name="issues-with-credentials"></a>Problémy s přihlašovacími údaji

Microsoft identity platform a tok přihlašovacích údajů klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) popisuje, jak naprogramovat přímo proti udělení toku přihlašovacích údajů klienta OAuth 2.0.

**Jak můžu spravovat heslo aplikace nebo přihlašovací údaje k certifikátu?**

V rozhraní příkazového řádku Azure můžete pomocí přihlašovacích údajů [aplikace az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) odstranit, zobrazit seznam nebo resetovat heslo nebo přihlašovací údaje k certifikátu aplikace.

**Jak uživatelé resetují svá hesla?**

Aby si [uživatelé](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mohli resetovat hesla, musí se zaregistrovat k samoobslužné resetování hesla. Jakmile se uživatel zaregistroval, může podle pokynů v tomto článku resetovat svoje heslo: Resetování pracovního nebo [školního hesla](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Jak uživatelé změní svá hesla?**

Uživatelé mohou podle pokynů v tomto článku změnit hesla: [Jak změnit heslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Taky [mohou spravovat hesla aplikací pro dvoukrokové ověření](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Při změně nebo resetování hesla se mému uživateli zobrazí chyba.**

Tento odkaz poskytne informace o běžných problémech, které mohou nastat, když se uživatel snaží resetovat heslo: Běžné problémy a [jejich řešení.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mám problém s resetováním hesla uživatele**

- Ujistěte se, že máte oprávnění k resetování hesel. *Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.* Globální správci můžou resetovat hesla dalších privilegovaných správců.

- Ujistěte se, že rozumíte licenčním požadavkům:

  - Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci:
    - **Jenom uživatelé cloudu** – všechny placené skladové Office 365 (O365) nebo Azure AD Basic
    - **Cloud a/nebo** místní uživatelé – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
    - Další informace o licenčních požadavcích najdete v tématu Licenční požadavky pro samoobslužné resetování [hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Pokud chcete resetovat heslo uživatele, najděte ho ve službě Azure AD. Potom v okně přehledu pro tohoto uživatele klikněte na tlačítko Resetovat heslo.

**Tlačítko pro resetování hesla je šedé**

Nejste oprávněni **resetovat** hesla tohoto uživatele. *Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.* Globální správci můžou resetovat hesla dalších privilegovaných správců.

**Nevidím okno pro resetování hesla**

K resetování hesel nejste oprávněni. *Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.* Globální správci můžou resetovat hesla dalších privilegovaných správců.

**V resetování hesla nevidím okno místní integrace**

- Okno místní integrace se zobrazuje jenom v hybridních prostředích, což znamená, že k manipulaci s hesly místního uživatele používáte zpětný zápis hesla.

- Tento list se zobrazí, pokud:

  - Nepou3/4ít zpětný zápis hesla
  - Došlo k problému s instalací nebo připojením zpětného zápisu hesla.
  - Došlo k problému s instalací nebo připojením služby Azure AD Připojení
  - Další kroky pro řešení problémů s zpětným zápisem hesla najdete v tématu Řešení potíží se zpětným [zápisem hesla.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nevím, jak resetovat heslo uživatele**

1. Přihlaste se k portálu Azure portal jako příslušný správce.
2. Přejděte do okna **Uživatelé a skupiny** a vyberte Všichni **uživatelé**.
3. V seznamu vyberte uživatele.
4. U vybraného uživatele vyberte **Přehled a** na panelu příkazů vyberte **Resetovat heslo**.
5. Vyberte tlačítko **Resetovat** heslo a postupujte podle pokynů na obrazovce.
    - Resetuje se jenom prostřednictvím zpětného **zápisu** hesla pro podporu portálu Azure Portal.

**Resetování hesla místního uživatele z portálu Office 365 Admin nebo mobilní aplikace Office 365 ale uživatel se pořád nemůže přihlásit**

Zpětný zápis hesla není na tomto portálu podporovaný. Resetujte heslo uživatele znovu na portálu Azure Portal.
