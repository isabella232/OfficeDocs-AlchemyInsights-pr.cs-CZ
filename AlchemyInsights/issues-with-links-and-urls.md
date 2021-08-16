---
title: Problémy s odkazy a adresami URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054791"
---
# <a name="issues-with-links-and-urls"></a>Problémy s odkazy a adresami URL

Přesměrování URI/reply a adres URL (oba výrazy jsou vzájemně zaměňovatelné) jsou adresy URL používané platformou Microsoft identity k vrácení tokenů požadovaných aplikací. Další informace o těchto URL adresách najdete v následujících článcích:

- [Toky ověřování a scénáře aplikací](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informace o přesměrováních URI na **stránce registrace aplikace** pro každý scénář.
- [Omezení a limity pro přesměrování adresy URL nebo identifikátor URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nevím, jak zaregistrovat správné přesměrování URI nebo URL pro mou aplikaci.**

Pokud se při přihlášení pomocí Vámi vyvíjené aplikace zobrazí dialog pro přihlášení **AADSTS50011: Adresa URL zadaná v žádosti neodpovídá adresám URL odpovědí nakonfigurovaných pro aplikace<your app ID>**, budete muset přidat do registrace vaší aplikace, URI přesměrování, který použil váš kód v žádosti o tokeny na platformě Microsoft Identity.

Pokud chcete přidat adresu URL, jděte na kartu **Autentifikace** na vaší **stránce registrace aplikace** na stránce Azure portal a přidejte položku do sekce **Přesměrovat URI** Hodnota, kterou potřebujete zadat, závisí na typu aplikace, kterou budete budovat, jak je popsáno níže:

- U jedno stránkových aplikací a webových aplikací se jako adresa URL odpovědi používá adresa URL vaší aplikace. Podívejte se [na jednostránkovou registraci](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) nebo [zaregistrujte webovou aplikaci pomocí Azure Portal.](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Hodnota, kterou si budete muset zvolit v desktopových aplikacích, závisí na:
    - platformě (MacOS se liší od Windows a Linuxu)
    - způsobu získání tokenu (interaktivně s tokem kódu zařízení, s Integrovaným Ověřováním Windows [IWA] nebo s uživatelským jménem a heslem).
    Podrobnosti najdete v [Desktopové aplikace – Registrace aplikace – Přesměrovat URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Identifikátor URI přesměrování v mobilních aplikacích závisí na:
    - platformě (iOS/Android/UWP)
    - Informaci používané k vytvoření aplikace, jako je ID svazku v iOS, název balíčku a hash podpis na Androidu, registrace aplikace na Azure portal vám pomůže. Podrobnosti najdete na [Platformě konfigurace a přesměrování identifikátorech URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Webová rozhraní API a některé tiché způsoby získání tokenů (IWA a uživatelské jméno a heslo) nevyžadují identifikátor URI přesměrování.

**Nasadil(a) jsem webovou aplikaci a když jsem otestoval(a) nasazenou aplikaci, zobrazí se zpráva o neshodě adresy URL**

Přidejte URI přesměrování pro všechna umístění, ve kterých webovou aplikaci nasazujete. Další informace najdete v [Registrace webové aplikace pomocí Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Přidejte URI přesměrování do umístění hned po nasazení aplikace v tomto umístění.

**Nemůžu zaregistrovat dost adres URL pro odpovědi**

Jste ISV a máte jednu nebo několik přesměrování URI pro každého zákazníka. Chcete migrovat z ADAL/Azure AD v1.0 na MSAL/platformu Microsoftu Identity a dosáhnete [maximálního počtu přesměrování URI ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Vyřešíte to [přidáním přesměrování URI do Service Principal](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) které odpovídají jednotlivým zákazníkům.
