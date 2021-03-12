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
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707875"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="0fd64-102">Problémy s odkazy a adresami URL</span><span class="sxs-lookup"><span data-stu-id="0fd64-102">Issues with links and URLs</span></span>

<span data-ttu-id="0fd64-103">Přesměrování URI/reply a adres URL (oba výrazy jsou vzájemně zaměňovatelné) jsou adresy URL používané platformou Microsoft identity k vrácení tokenů požadovaných aplikací.</span><span class="sxs-lookup"><span data-stu-id="0fd64-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="0fd64-104">Další informace o těchto URL adresách najdete v následujících článcích:</span><span class="sxs-lookup"><span data-stu-id="0fd64-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="0fd64-105">[Toky ověřování a scénáře aplikací](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informace o přesměrováních URI na **stránce registrace aplikace** pro každý scénář.</span><span class="sxs-lookup"><span data-stu-id="0fd64-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="0fd64-106">Omezení a limity pro přesměrování adresy URL nebo identifikátor URI</span><span class="sxs-lookup"><span data-stu-id="0fd64-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="0fd64-107">**Nevím, jak zaregistrovat správné přesměrování URI nebo URL pro mou aplikaci.**</span><span class="sxs-lookup"><span data-stu-id="0fd64-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="0fd64-108">Pokud se při přihlášení pomocí Vámi vyvíjené aplikace zobrazí dialog pro přihlášení **AADSTS50011: Adresa URL zadaná v žádosti neodpovídá adresám URL odpovědí nakonfigurovaných pro aplikace<your app ID>**, budete muset přidat do registrace vaší aplikace, URI přesměrování, který použil váš kód v žádosti o tokeny na platformě Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="0fd64-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="0fd64-109">Pokud chcete přidat adresu URL, jděte na kartu **Autentifikace** na vaší **stránce registrace aplikace** na stránce Azure portal a přidejte položku do sekce **Přesměrovat URI**</span><span class="sxs-lookup"><span data-stu-id="0fd64-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="0fd64-110">Hodnota, kterou potřebujete zadat, závisí na typu aplikace, kterou budete budovat, jak je popsáno níže:</span><span class="sxs-lookup"><span data-stu-id="0fd64-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="0fd64-111">U jedno stránkových aplikací a webových aplikací se jako adresa URL odpovědi používá adresa URL vaší aplikace.</span><span class="sxs-lookup"><span data-stu-id="0fd64-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="0fd64-112">Podívejte se [na jednostránkovou registraci](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) nebo [zaregistrujte webovou aplikaci pomocí Azure Portal.](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="0fd64-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="0fd64-113">Hodnota, kterou si budete muset zvolit v desktopových aplikacích, závisí na:</span><span class="sxs-lookup"><span data-stu-id="0fd64-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="0fd64-114">platformě (MacOS se liší od Windows a Linuxu)</span><span class="sxs-lookup"><span data-stu-id="0fd64-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="0fd64-115">způsobu získání tokenu (interaktivně s tokem kódu zařízení, s Integrovaným Ověřováním Windows [IWA] nebo s uživatelským jménem a heslem).</span><span class="sxs-lookup"><span data-stu-id="0fd64-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="0fd64-116">Podrobnosti najdete v [Desktopové aplikace – Registrace aplikace – Přesměrovat URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="0fd64-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="0fd64-117">Identifikátor URI přesměrování v mobilních aplikacích závisí na:</span><span class="sxs-lookup"><span data-stu-id="0fd64-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="0fd64-118">platformě (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="0fd64-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="0fd64-119">Informaci používané k vytvoření aplikace, jako je ID svazku v iOS, název balíčku a hash podpis na Androidu, registrace aplikace na Azure portal vám pomůže.</span><span class="sxs-lookup"><span data-stu-id="0fd64-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="0fd64-120">Podrobnosti najdete na [Platformě konfigurace a přesměrování identifikátorech URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="0fd64-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="0fd64-121">Webová rozhraní API a některé tiché způsoby získání tokenů (IWA a uživatelské jméno a heslo) nevyžadují identifikátor URI přesměrování.</span><span class="sxs-lookup"><span data-stu-id="0fd64-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="0fd64-122">**Nasadil(a) jsem webovou aplikaci a když jsem otestoval(a) nasazenou aplikaci, zobrazí se zpráva o neshodě adresy URL**</span><span class="sxs-lookup"><span data-stu-id="0fd64-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="0fd64-123">Přidejte URI přesměrování pro všechna umístění, ve kterých webovou aplikaci nasazujete.</span><span class="sxs-lookup"><span data-stu-id="0fd64-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="0fd64-124">Další informace najdete v [Registrace webové aplikace pomocí Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="0fd64-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="0fd64-125">Přidejte URI přesměrování do umístění hned po nasazení aplikace v tomto umístění.</span><span class="sxs-lookup"><span data-stu-id="0fd64-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="0fd64-126">**Nemůžu zaregistrovat dost adres URL pro odpovědi**</span><span class="sxs-lookup"><span data-stu-id="0fd64-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="0fd64-127">Jste ISV a máte jednu nebo několik přesměrování URI pro každého zákazníka.</span><span class="sxs-lookup"><span data-stu-id="0fd64-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="0fd64-128">Chcete migrovat z ADAL/Azure AD v1.0 na MSAL/platformu Microsoftu Identity a dosáhnete [maximálního počtu přesměrování URI ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="0fd64-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="0fd64-129">Vyřešíte to [přidáním přesměrování URI do Service Principal](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) které odpovídají jednotlivým zákazníkům.</span><span class="sxs-lookup"><span data-stu-id="0fd64-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
