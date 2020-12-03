---
title: Povolení zpětného zápisu hesel v Azure AD Connect
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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560433"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Povolení zpětného zápisu hesel v Azure AD Connect

Pokud chcete povolit samoobslužný zápis resetování hesla, nejdřív v Azure AD Connect povolte možnost zpětný zápis. Ze svého serveru Azure AD Connect udělejte toto:

1. Přihlaste se k serveru Azure AD Connect a spusťte Průvodce konfigurací **Azure AD Connect** .
2. Na **úvodní** stránce klikněte na **Konfigurovat**.
3. Na stránce **Další úkoly** vyberte **přizpůsobit možnosti synchronizace** a pak klikněte na **Další**.
4. Na stránce **Connect to Azure AD** zadejte přihlašovací údaje globálního správce pro tenanta Azure a klikněte na **Další**.
5. Na stránkách **připojit adresáře** a filtrování **domény nebo organizační jednotky** klikněte na **Další**.
6. Na stránce **volitelné funkce** zaškrtněte políčko u položky **zpětný zápis hesla** a klikněte na **Další**.
7. Na stránce **připraveno ke konfiguraci** klikněte na **Konfigurovat** a počkejte, až se proces dokončí.
8. Po dokončení konfigurace klikněte na **konec**.

Když v Azure AD Connect povolíte zpětný zápis hesla, nakonfigurujte Azure AD SSPR pro zpětný zápis.  Pokud chcete povolit zpětný zápis hesel v SSPR, postupujte takto:

1. Přihlaste se k portálu Azure pomocí účtu globálního správce.
2. Vyhledejte a vyberte **Azure Active Directory**, klikněte na **resetovat heslo** a potom klikněte na **Místní integrace**.
3. Nastavte možnost pro **zápis hesel do místního adresáře?** na **Ano**.
4. Nastavte možnost **Povolit uživatelům odemknutí účtů, aniž byste museli resetovat heslo?** **Yes**
5. Až budete připraveni, klikněte na **Uložit**.

Další informace najdete v tématu [Povolení automatického obnovení hesla služby Azure Active Directory pro místní prostředí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Pokud správce resetuje heslo uživatele na portálu Azure, bude se heslo zapisovat zpátky do místního počítače, pokud je tento uživatel v jeho synchronizaci. Tato funkce není momentálně podporovaná na portálu pro správu Office.