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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069957"
---
# <a name="conditional-access-issues"></a>Problémy s podmíněným přístupem

**Řešení problémů s diagnostickou chybou přihlášení**

Pomocí nástroje Diagnostika přihlášení můžete rychle zjistit, co se stalo, nebo diagnostikovat problémy související s [přihlášením uživatele:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Spusťte diagnostiku přihlášení.
1. Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, čase přihlášení, ID žádosti nebo ID korelace.
1. Zkontrolujte diagnostické výsledky s podrobnostmi o tom, co se stalo, a jaké akce můžete provést k provedení změn (pokud jsou potřeba nějaké změny).

**Postup řešení potíží s přihlášením** 

1. Přejděte na přihlašovací stránku Azure AD.
1. Filtrování přihlášení podle uživatele, časového rozsahu, aplikace, stavu, klientské aplikace atd.
1. Vyberte přihlašovací událost a zobrazte kartu Podmíněný přístup a podívejte se, které zásady byly vyhodnocovány.
1. Kliknutím na řádek zásady zobrazíte podrobnosti zásad a pochopíte, proč se zásady použily.

**Nástroje pro řešení potíží se zásadou podmíněného přístupu**

- Režim jen pro sestavy umožňuje vyhodnotit zásadu, aniž by to ovlivnilo uživatele.
- Nástroj What-if umožňuje simulovat události přihlášení a zobrazit, které zásady platí.
- Přehledy a vytváření sestav zobrazuje dopad jednotlivých zásad v reálném čase.

**Zásady ochrany podle směrného plánu**

Zásady ochrany podle směrného plánu jsou zastaralé. Už se nenucuje a brzy se odebere z portálu Azure Portal. Doporučujeme povolit výchozí [nastavení zabezpečení](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Další informace o podmíněném přístupu najdete v těchto článku:

[Doporučené postupy pro podmíněný přístup v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Podmínky v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ovládací prvky v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Umístění v podmíněném přístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
