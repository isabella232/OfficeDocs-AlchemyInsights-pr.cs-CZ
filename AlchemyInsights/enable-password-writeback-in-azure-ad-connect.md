---
title: Povolení zpětného zápisu hesla ve službě Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204618"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Povolení zpětného zápisu hesla ve službě Azure AD Connect

Chcete-li povolit zpětný zápis pro obnovení samoobslužného hesla, nejprve povolte možnost zpětného zápisu ve službě Azure AD Connect. Na serveru Azure AD Connect proveďte následující kroky:

1. Přihlaste se k serveru Azure AD Connect a spusťte průvodce konfigurací **Azure AD Connect.**
2. Na **úvodní** stránce klepněte na tlačítko **Konfigurovat**.
3. Na stránce **Další úkoly** vyberte **Přizpůsobit možnosti synchronizace**a klepněte na tlačítko **Další**.
4. Na stránce **Připojit k Azure AD** zadejte pověření globálního správce pro vašeho klienta Azure a klikněte na Další.
5. Na stránkách **Connect directories** a **Domain/OU** filtering klepněte na tlačítko **Další**.
6. Na stránce **Volitelné funkce** zaškrtněte políčko vedle **možnosti Zpětný zápis hesla** a klepněte na tlačítko **Další**.
7. Na stránce **Připraveno ke konfiguraci** klikněte na **Konfigurovat** a počkejte na dokončení procesu.
8. Po dokončení konfigurace klepněte na tlačítko **Ukončit**.

Když je ve Službě Azure AD Connect povolen zpětný zápis hesla, nakonfigurujte azure ad ssdr pro zpětný zápis.  Chcete-li povolit zpětný zápis hesla v sspr, proveďte následující kroky:

1. Přihlaste se k portálu Azure pomocí účtu globálního správce.
2. Vyhledejte a vyberte **Azure Active Directory**, klikněte na **Obnovit heslo**a pak zvolte Místní **integrace**.
3. Nastavit možnost **pro zápis hesel do místního adresáře?** **Yes**
4. Nastavit možnost **Povolit uživatelům odemknout účty bez resetování hesla?** **Yes**
5. Až budete připraveni, klepněte na tlačítko **Uložit**.

Další informace naleznete v tématu [Povolení samoobslužného zpětného zápisu hesla služby Azure Active Directory do místního prostředí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
