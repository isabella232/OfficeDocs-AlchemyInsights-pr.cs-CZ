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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404366"
---
# <a name="authentication-app"></a>Aplikace pro ověřování

Pokud jste globální správce, můžete rychle zjistit, co se stalo, nebo diagnostikovat problémy související s přihlášením uživatele pomocí [nástroje Diagnostika přihlášení](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Spusťte diagnostiku kliknutím na tlačítko Spustit[diagnostiku.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, čase přihlášení, ID žádosti nebo ID korelace.
1. Zkontrolujte diagnostické výsledky s podrobnostmi o tom, co se stalo, a jaké akce můžete provést, pokud jsou potřeba nějaké změny.

**Zkontrolujte scénář, který se použije:**

1. Pokud se uživateli v aplikaci Microsoft Authenticator nezobrazují nabízená oznámení, ověřte, že se nezobrazují pod blokovaným uživatelům MFA, jak je popsáno v článku Blokování a [odblokování uživatelů](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Pokud uživatel není pro MFA zablokovaný, ale neobdrží nabízené oznámení, může otevřít aplikaci Microsoft Authenticator, která vyžádá čekající žádosti o schválení.
1. Jako alternativní způsob přihlášení může uživatel taky kliknout na Přihlásit se jiným způsobem a zvolit použití ověřovacího kódu z mobilní aplikace.
1. Aplikace Microsoft Authenticator je jedinou dostupnou metodou pro mnoho uživatelů. [Přečtěte si další informace o výchozích](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)nastaveních zabezpečení , nejčastější dotazy k [aplikacím Authenticator,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) kde najdete nejčastější dotazy a jak je vyřešit.
 
**Doporučená videa**

[Jak nastavit aplikaci Authenticator na novém telefonu (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
