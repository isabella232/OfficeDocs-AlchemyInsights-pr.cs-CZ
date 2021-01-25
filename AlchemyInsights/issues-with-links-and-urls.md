---
title: Problémy s odkazy a adresami URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974228"
---
# <a name="issues-with-links-and-urls"></a>Problémy s odkazy a adresami URL

Adresy URL pro přesměrování adres URI a odpovědí (jsou oba výrazy zaměnitelné) jsou adresy URL používané platformou Microsoft identity k vrácení tokenů požadovaných aplikací. Informace o těchto adresách URL najdete v následujících článcích:

- [Postupy ověřování a scénáře aplikací](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informace o identifikátorech URI přesměrování v **registrační stránce aplikací** pro jednotlivé scénáře.
- [Omezení a omezení adresy URL pro přesměrování podle identifikátoru URI/odpovědi](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nevím, jak registrovat přihlašovací adresu URL pro moje aplikace.**

Když se přihlásíte pomocí aplikace, kterou vyvíjíte, pokud se v dialogovém okně pro přihlášení zobrazí **AADSTS50011: adresa URL odpovědi zadaná v žádosti neodpovídá adresám URL pro odpověď konfigurovaným pro <your app ID> aplikaci**, budete muset přidat do registrace aplikace, identifikátor URI přesměrování, který váš kód použil v žádosti o token na platformě Microsoft identity.

Pokud chcete přidat adresu URL odpovědi, přejděte na kartě **ověřování** na **registrační stránce aplikace** na portálu Azure a přidejte položku do oddílu **redirect URI** . Přesměrované identifikátory URI jsou zadané (web nebo mobilní síť). Zadaná hodnota závisí na typu aplikace, kterou vytváříte, jak je popsáno níže:

- U aplikací s jedním stránkou a webových aplikací je adresa URL odpovědi v aplikaci. Viz [registrace jedné stránky](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) nebo registrace [aplikace webové aplikace pomocí portálu Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- U desktopových aplikací je třeba, aby byla hodnota, kterou chcete vybrat, závislá:
    - Platforma (MacOS se liší od systému Windows nebo Linux)
    - způsob, jakým získáváte token (interaktivně pomocí integrovaného ověřování systému Windows [IWA] nebo pomocí uživatelského jména a hesla).
    Podrobnosti najdete v tématu [desktopové aplikace – registrace aplikace – URi přesměrování](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris) .
- U mobilních aplikací závisí identifikátor URI přesměrování na:
    - Platform (iOS/Android/UWP)
    - informace použité k sestavování aplikací, jako je ID sady v iOS, a název balíčku a hodnota hash podpisu na Androidu vám to pomůže. Podrobnosti najdete v tématu [konfigurace platformy a identifikátory URI přesměrování](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Webová rozhraní API a některé z bezobslužných způsobů získání tokenů (IWA a username/Password) nevyžadují identifikátor URI přesměrování.

**Po nasazení webové aplikace a při testování nasazené aplikace se zobrazuje zpráva o neshodě adresy URL odpovědi**

Přidejte identifikátory URI pro přesměrování pro všechna umístění, kde nasazujete webovou aplikaci. Další informace najdete v článku [Registrace aplikace webové aplikace pomocí portálu Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Přidejte URI pro přesměrování pro umístění hned po nasazení aplikace v daném umístění.

**Nemůžu zaregistrovat dostatečný počet adres URL pro odpovědi**

Jste prodejcem ISV a máte jeden nebo několik identifikátorů URI přesměrování pro každého zákazníka svého. Chcete migrovat z ADAL/Azure AD v 1.0 na MSAL/The Microsoft Identity Platform a zasáhnete [maximální počet identifikátorů URI přesměrování](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Tento problém vyřešíte [přidáním identifikátorů URI pro přesměrování k instančním objektům](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , které odpovídají jednotlivým zákazníkům.
