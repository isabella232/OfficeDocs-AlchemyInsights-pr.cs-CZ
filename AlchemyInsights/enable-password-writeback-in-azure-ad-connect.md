---
title: Povolení zpětného zápisu hesla v Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093348"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Povolení zpětného zápisu hesla v Azure AD Connect

Pokud chcete povolit samoobslužné resetování zápisu hesel, na prvním místě povolte možnost zpětného zápisu v Azure AD Connect. Na serveru Azure AD Connect proveďte následující kroky:

1. Přihlaste se k serveru Azure AD Connect a spusťte **průvodce konfigurací Azure AD Connect.**
2. Na úvodní **stránce** klikněte na **Konfigurovat.**
3. Na stránce **Další úkoly** vyberte Přizpůsobit **možnosti synchronizace** a potom klikněte na **Další.**
4. Na stránce **Připojit k Azure AD** zadejte přihlašovací údaje globálního správce pro vašeho tenanta Azure a klikněte na **Další.**
5. Na **stránkách připojení adresářů** a filtrování **domény a OU** klikněte na **Další.**
6. Na stránce **Volitelné funkce** zaškrtněte políčko  vedle možnosti Zpětný zápis hesla a klikněte na **Další.**
7. Na stránce **Ready to configure** (Připraveno ke konfiguraci) klikněte na **Configure** (Konfigurovat) a počkejte, až proces skončí.
8. Až uvidíte dokončení konfigurace, klikněte na **Konec.**

Pokud je v Azure AD Connect povolený zpětný zápis hesel, nakonfigurujte Azure AD SSPR pro zpětný zápis.  Pokud chcete v SSPR povolit zpětný zápis hesel, proveďte následující kroky:

1. Přihlaste se k portálu Azure Portal pomocí účtu globálního správce.
2. Vyhledejte a vyberte **Azure Active Directory, klikněte** na **Resetování hesla** a potom klikněte na místní **integraci.**
3. Nastavte možnost pro **zapisování** hesel do místního adresáře? na **Ano.**
4. Nastavte možnost povolit **uživatelům odemykání účtů bez resetování jejich hesla?** **Nastavte Ano.**
5. Až budete připravení, klikněte na **Uložit.**

Další informace najdete v článku o povolení samoobslužných resetování hesel pro Azure Active Directory do [místního prostředí.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)

> [!NOTE]
>  Když správce resetuje heslo uživatele na portálu Azure Portal a tento uživatel je federovaný nebo synchronizovaný s hodnotou hash hesel, heslo se zapište zpátky do místního prostředí. Tato funkce vyžaduje licenci Azure Premium (P1 nebo P2) a není momentálně podporovaná na portálu pro správu Office.
