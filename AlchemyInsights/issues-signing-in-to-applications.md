---
title: Problémy s přihlášením k aplikacím
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900802"
---
# <a name="issues-signing-in-to-applications"></a>Problémy s přihlášením k aplikacím

Pokud chcete zjistit příčinu nebo diagnostikovat problémy související s přihlašováním uživatelů, postupujte takto:

1. Spusťte diagnostický nástroj pro [přihlášení](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, času přihlášení, ID žádosti nebo ID korelace.
3. Prohlédněte si výsledky diagnostických nástrojů s podrobnostmi o tom, co se stalo a jaké akce můžete provádět, pokud jsou potřeba.

Tady jsou některé běžné problémy, se kterými se můžete setkat při přihlašování k aplikacím:

1. Vy nebo uživatel **dokončí přihlášení Azure AD, ale zobrazuje se neočekávaná výzva** – Podívejte se na články [neočekávaného souhlasu při přihlášení k aplikaci](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) a [neočekávané chybě při provádění souhlasu s aplikací](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Vy nebo uživatel jste se **k aplikaci přihlásili přímo, ale nemůžete se k němu přihlásit pomocí odkazu deeplink na vlastním portálu nebo na panelu pro přístup**: řešení potíží s [přihlášením k aplikaci z Azure AD moje aplikace](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Vy nebo uživatel **dokončili přihlášení Azure AD, ale aplikace zobrazí chybovou zprávu a neumožní uživateli dokončit přihlašování**. problém je, že aplikace nepřijala odpověď, kterou služba Azure AD vydala. Při řešení potíží postupujte podle [těchto kroků](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) .
4. Vy nebo uživatel se **nemůžete přihlásit k aplikaci negalerie, která je nakonfigurovaná pro heslo**, postupujte podle pokynů v [těchto krocích](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) .
5. Vy nebo uživatel se **nemůžete přihlásit k aplikaci Galerie Azure AD konfigurovanou pro heslo pomocí jednotného přihlašování**: postupujte podle [těchto pokynů](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) .
6. Vy nebo uživatel se **nemůžete přihlásit k aplikaci Microsoftu**: postupujte podle [těchto pokynů](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) .
7. Vy nebo uživatel se **nemůžete přihlásit k aplikaci negalerie, která je nakonfigurovaná pro federované jednotné přihlašování**: postupujte podle [těchto pokynů](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) .
8. Vy nebo uživatel se **nemůžete přihlásit k aplikaci Galerie Azure AD konfigurovanou pro federované jednotné přihlašování**: postupujte podle [těchto pokynů](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) .
9. Vy nebo uživatel se **nemůžete přihlásit ke vlastní aplikaci**: řešení potíží podle [těchto kroků](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) .
10. Vy nebo uživatel se **nemůžete přihlásit do místní aplikace pomocí proxy Azure AD** [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)

