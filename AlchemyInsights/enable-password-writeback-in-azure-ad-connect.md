---
title: Povolení zpětného zápisu hesla v Azure AD Connect
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
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814005"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Povolení zpětného zápisu hesla v Azure AD Connect

Pokud chcete povolit samoobslužný zpětný zápis pro resetování hesla, povolte nejdřív možnost zpětného zápisu v Azure AD Connect. Na serveru Azure AD Connect proveďte následující kroky:

1. Přihlaste se k serveru Azure AD Connect a spusťte průvodce konfigurací **Azure AD Connect.**
2. Na úvodní **stránce** klikněte na **Konfigurovat.**
3. Na stránce **Další úkoly** vyberte Přizpůsobit **možnosti synchronizace** a potom klikněte na **Další.**
4. Na stránce **Připojit se k Azure AD** zadejte přihlašovací údaje globálního správce pro vašeho tenanta Azure a klikněte na **Další.**
5. Na **stránkách Propojte adresáře** a **filtrování domény/OU** klikněte na **Další.**
6. Na stránce **Volitelné** funkce zaškrtněte políčko vedle položky Zpětný zápis hesla a **klikněte** na **Další.**
7. Na stránce **Ready to configure** (Připraveno ke konfiguraci) klikněte na **Configure** (Konfigurovat) a počkejte na dokončení procesu.
8. Až uvidíte dokončení konfigurace, klikněte na **Ukončit.**

S povoleným zpětným zápisem hesel v Azure AD Connect nakonfigurujte Azure AD SSPR pro zpětný zápis.  Pokud chcete povolit zpětný zápis hesel v SSPR, postupujte takto:

1. Přihlaste se k webu Azure Portal pomocí účtu globálního správce.
2. Vyhledejte a vyberte **Azure Active Directory,** klikněte na **Resetování hesla** a potom klikněte na Místní **integrace.**
3. Nastavte možnost Pro zápis hesel zpět do místního **adresáře?** na **Ano**.
4. Nastavte možnost Povolit **uživatelům odemknout účty bez resetování hesla?** na **Ano**.
5. Až budete připravení, klikněte na **Uložit.**

Další informace najdete v tématu [Povolení samoobslužných](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)zpětných zápisů resetování hesla v Azure Active Directory do místního prostředí .

> [!NOTE]
>  Když správce resetuje heslo uživatele na portálu Azure Portal, pokud je tento uživatel federovaný nebo se synchronizuje hodnota hash hesla, heslo se zapisuje zpátky do místního prostředí. Tato funkce vyžaduje licenci Azure Premium (P1 nebo P2) a momentálně není podporovaná na portálu pro správu Office.
