---
title: Aplikace pro ověřování
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082935"
---
# <a name="authentication-app"></a>Aplikace pro ověřování

Pokud jste globální správce, můžete rychle zjistit, co se stalo, nebo diagnostikovat problémy související s přihlášením uživatele pomocí [nástroje Diagnostika přihlášení](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Spusťte diagnostiku kliknutím na tlačítko Spustit[diagnostiku.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, čase přihlášení, ID žádosti nebo ID korelace.
1. Zkontrolujte diagnostické výsledky s podrobnostmi o tom, co se stalo, a jaké akce můžete provést, pokud jsou potřeba nějaké změny.

**Zkontrolujte scénář, který se použije:**

1. Pokud uživatel v aplikaci Microsoft Authenticator nedosáhá nabízených oznámení, ověřte, že se nezobrazují pod blokovaným uživatelům MFA, jak je popsáno v článku Blokování a [odblokování uživatelů](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Pokud uživatel není pro MFA zablokovaný, ale neobdrží nabízené oznámení, může otevřít aplikaci Microsoft Authenticator, která vyžádá čekající žádosti o schválení.
1. Jako alternativní způsob přihlášení může uživatel taky kliknout na Přihlásit se jiným způsobem a zvolit použití ověřovacího kódu z mobilní aplikace.
1. Aplikace Microsoft Authenticator je jedinou dostupnou metodou pro mnoho uživatelů. [Přečtěte si další informace o výchozích](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)nastaveních zabezpečení , Authenticator nejčastější dotazy k [aplikacím](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) a jak je vyřešit.
 
**Doporučená videa**

[Jak nastavit Authenticator na novém telefonu (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
