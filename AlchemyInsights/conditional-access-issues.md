---
title: Problémy s podmíněným přístupem
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014746"
---
# <a name="conditional-access-issues"></a>Problémy s podmíněným přístupem

**Řešení problémů s diagnostickou pro přihlášení**

Pomocí [diagnostických nástrojů pro přihlášení](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)můžete rychle zjistit, co se stalo nebo jak diagnostikovat problémy související s přihlašováním:

1. Spusťte diagnostický nástroj pro přihlášení.
1. Najděte událost, kterou chcete analyzovat, zadáním informací o uživateli, aplikaci, času přihlášení, ID žádosti nebo ID korelace.
1. Prohlédněte si výsledky diagnostických nástrojů s podrobnostmi o tom, co se stalo a jaké akce můžete provést, abyste udělali změny (pokud jsou potřeba nějaké změny).

**Řešení potíží s přihlášením** 

1. Přejděte na přihlašovací stránku Azure AD.
1. Filtrovat přihlášení podle uživatele, časového rozsahu, aplikace, stavu, klientské aplikace atd.
1. Vyberte přihlašovací událost a zobrazte kartu pro podmíněný přístup a zjistěte, které zásady byly vyhodnoceny.
1. Kliknutím na řádek zásad zobrazte podrobnosti o zásadách a zjistěte, proč to byla použita.

**Nástroje pro řešení potíží s zásadou podmíněného přístupu**

- Režim pouze sestavy umožňuje vyhodnotit zásady bez ovlivnění uživatelů.
- Nástroj citlivosti umožňuje simulovat události přihlášení a zjistit, které zásady se používají.
- V sešitě přehledů a sestav se zobrazuje dopad jednotlivých zásad v reálném čase.

**Zásady ochrany základní úrovně**

Zásady ochrany podle směrného plánu byly zastaralé. Už se nevynucují a brzy se odeberou z Azure Portalu. Doporučujeme povolit [výchozí nastavení zabezpečení](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Další informace o podmíněném přístupu najdete v těchto tématech:

[Osvědčené postupy pro podmíněný přístup v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Podmínky v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ovládací prvky v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Umístění v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
