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
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709720"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Povolení zpětného zápisu hesel v Azure AD Connect

Pokud chcete povolit samoobslužný zápis resetování hesla, nejdřív v Azure AD Connect povolte možnost zpětný zápis. Ze svého serveru Azure AD Connect udělejte toto:

1. Přihlaste se k serveru Azure AD Connect a spusťte Průvodce konfigurací **Azure AD Connect** .
2. Na **úvodní** stránce klikněte na **Konfigurovat**.
3. Na stránce **Další úkoly** vyberte **přizpůsobit možnosti synchronizace**a pak klikněte na **Další**.
4. Na stránce **Connect to Azure AD** zadejte přihlašovací údaje globálního správce pro tenanta Azure a klikněte na další.
5. Na stránkách **připojit adresáře** a filtrování **domény nebo organizační jednotky** klikněte na **Další**.
6. Na stránce **volitelné funkce** zaškrtněte políčko u položky **zpětný zápis hesla** a klikněte na **Další**.
7. Na stránce **připraveno ke konfiguraci** klikněte na **Konfigurovat** a počkejte, až se proces dokončí.
8. Po dokončení konfigurace klikněte na **konec**.

Když v Azure AD Connect povolíte zápis hesel, teď nakonfigurujte Azure AD SSPR pro zpětný zápis.  Pokud chcete povolit zpětný zápis hesel v SSPR, postupujte takto:

1. Přihlaste se k portálu Azure pomocí účtu globálního správce.
2. Vyhledejte a vyberte **Azure Active Directory**, klikněte na **resetovat heslo**a pak zvolte **Místní integrace**.
3. Nastavte možnost pro **zápis hesel do místního adresáře?** na **Ano**.
4. Nastavte možnost **Povolit uživatelům odemknutí účtů, aniž byste museli resetovat heslo?** **Yes**
5. Až budete připraveni, klikněte na **Uložit**.

Další informace najdete v tématu [Povolení automatického obnovení hesla služby Azure Active Directory pro místní prostředí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
