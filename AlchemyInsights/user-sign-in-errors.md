---
title: Chyby přihlášení uživatelů
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
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900790"
---
# <a name="user-sign-in-errors"></a>Chyby přihlášení uživatelů

**Řešení problémů s diagnostickou pro přihlášení**

Pokud chcete zjistit příčinu nebo diagnostikovat problémy související s přihlašováním uživatelů, postupujte takto:

1. Spusťte diagnostický nástroj pro [přihlášení](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Najděte událost, kterou chcete analyzovat, zadáním podrobností o uživateli, aplikaci, času přihlášení, ID žádosti nebo ID korelace.
3. Prohlédněte si výsledky diagnostických nástrojů s podrobnostmi o tom, co se stalo a jaké akce můžete provádět, pokud jsou potřeba.

**Hledáte informace o kódech chyb AADSTS, které jsou vraceny ze služby tokenů zabezpečení Azure Active Directory (STS)?** V [tomto článku](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) najdete popis AADSTS chyb, opravy a některá navrhovaná řešení.