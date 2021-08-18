---
title: Povolení zpětného zápisu hesel ve službě Azure AD Připojení
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325380"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Povolení zpětného zápisu hesel ve službě Azure AD Připojení

Pokud chcete povolit zpětný zápis pro samoobslužné resetování hesla, povolte nejdřív možnost zpětného zápisu v Azure AD Připojení. Na svém Připojení Azure AD proveďte následující kroky:

1. Přihlaste se k serveru Azure AD Připojení a spusťte Průvodce konfigurací **služby Azure AD Připojení** konfigurace.
2. Na úvodní **stránce** klikněte na **Konfigurovat.**
3. Na stránce **Další úkoly** vyberte Přizpůsobit **možnosti synchronizace** a potom klikněte na **Další.**
4. Na stránce **Připojení azure AD** zadejte přihlašovací údaje globálního správce pro vašeho tenanta Azure a klikněte na **Další.**
5. Na stránce **Připojení adresáře** a filtrování **domén/OU** klikněte na **Další.**
6. Na stránce **Volitelné** funkce zaškrtněte políčko vedle položky Zpětný zápis hesla a **klikněte** na **Další.**
7. Na stránce **Ready to configure** (Připraveno ke konfiguraci) klikněte na **Configure** (Konfigurovat) a počkejte na dokončení procesu.
8. Až uvidíte dokončení konfigurace, klikněte na **Ukončit.**

S povoleným zpětným zápisem hesel v Azure AD Připojení nakonfigurujte Azure AD SSPR pro zpětný zápis.  Pokud chcete povolit zpětný zápis hesel v SSPR, postupujte takto:

1. Přihlaste se k webu Azure Portal pomocí účtu globálního správce.
2. Vyhledejte a vyberte **Azure Active Directory**, klikněte na **Resetování hesla** a potom klikněte na **Místní integrace.**
3. Nastavte možnost Pro zápis hesel zpět do místního **adresáře?** na **Ano**.
4. Nastavte možnost Povolit **uživatelům odemknout účty bez resetování hesla?** na **Ano**.
5. Až budete připravení, klikněte na **Uložit.**

Další informace najdete v tématu Povolení Azure Active Directory samoobslužné zpětného zápisu hesla do [místního prostředí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

**Poznámka:** Když správce resetuje heslo uživatele na portálu Azure Portal, pokud je tento uživatel federovaný nebo se synchronizuje hodnota hash hesla, heslo se zapisuje zpátky do místního prostředí. Tato funkce vyžaduje licenci Azure Premium (P1 nebo P2) a momentálně není podporovaná na portálu Office správce.
