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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063598"
---
# <a name="issues-with-credentials"></a>Problémy s přihlašovacími údaji

Platforma identit Microsoft a tok přihlašovacích údajů klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) popisují, jak programovat přímo proti toku přihlašovacích údajů klienta OAuth 2.0.

**Jak můžu spravovat přihlašovací údaje aplikace pro heslo nebo certifikát?**

V Azure CLI můžete přihlašovací údaje [aplikace az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) použít k odstranění, vytvoření seznamu nebo resetování přihlašovacích údajů pro heslo aplikace nebo certifikát.

**Jak si uživatelé resetují hesla?**

Uživatelé se musí [před resetováním](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) hesel zaregistrovat k samoobslužné resetování hesla. Jakmile se uživatel zaregistroval, může si podle pokynů v tomto článku resetovat heslo: resetovat si pracovní nebo [školní heslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Jak si uživatelé změní hesla?**

Uživatelé mohou při změně hesla postupovat podle pokynů v tomto článku: Jak [si změnit heslo.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Mohou také [spravovat hesla aplikací pro dvoukroové ověření.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Při změně nebo resetování hesla se uživateli zobrazí chyba**

Tento odkaz poskytne informace o běžných problémech, které mohou nastat při pokusu uživatele o resetování hesla: Běžné problémy a [jejich řešení.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mám problém s resetováním uživatelského hesla**

- Ujistěte se, že máte oprávnění k resetování hesel. *Hesla uživatele můžou resetovat jenom globální správci a správci uživatelů.* Globální správci můžou taky resetovat hesla jiných privilegovaných správců.

- Ujistěte se, že rozumíte licenčním požadavkům:

  - Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci:
    - **Jenom cloudové uživatele** – všechny placené SKU Office 365 (O365) nebo Azure AD Basic
    - **Cloudové a místní** uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
    - Další informace o licenčních požadavcích najdete v článku o licenčních požadavcích pro samoobslužné resetování [hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Pokud chcete resetovat heslo uživatele, najděte uživatele v Azure AD. Pak v listu přehledu pro tohoto uživatele klikněte na tlačítko Resetovat heslo.

**Tlačítko pro resetování hesla se zobrazí šedě**

K resetování hesel **tohoto** uživatele nejste oprávněni. *Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.* Globální správci můžou taky resetovat hesla jiných privilegovaných správců.

**Nevidím list pro resetování hesla**

K resetování hesel máte oprávnění. *Hesla uživatele můžou resetovat jenom globální správci, hesla a správci uživatelů.* Globální správci můžou taky resetovat hesla jiných privilegovaných správců.

**Při resetování hesla nevidím místní integraci s listy**

- Místní integrace se zobrazuje jenom v hybridních prostředích, což znamená, že používáte k práci s hesly místních uživatelů zpětný zápis hesel.

- Tento list se nezkoumá, pokud:

  - Používáte bez zpětného zápisu hesla
  - Došlo k problému s instalací nebo připojením zpětného zápisu hesla
  - Došlo k problému s instalací nebo připojením služby Azure AD Connect.
  - Další kroky pro řešení problémů s zpětným zápisem hesla najdete v článku [Řešení potíží se zpětným zápisem hesla](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nevím, jak resetovat heslo uživatele**

1. Přihlaste se k portálu Azure Portal jako příslušný správce.
2. Přejděte do okna **Uživatelé a skupiny** a vyberte Všichni **uživatelé.**
3. Vyberte uživatele ze seznamu.
4. U vybraného uživatele vyberte **Přehled a** potom na panelu příkazů vyberte **Resetovat heslo.**
5. Vyberte tlačítko **Resetovat** heslo a postupujte podle pokynů na obrazovce.
    - Obnovení pouze prostřednictvím **zpětného zápisu** hesla pro podporu na portálu Azure Portal

**Resetování hesla místního uživatele z portálu pro správu Office 365 nebo mobilní aplikace Office 365, ale uživatel se pořád nemůže přihlásit**

Na tomto portálu se nepodporuje zpětný zápis hesel. Resetujte heslo uživatele znovu na portálu Azure Portal.
