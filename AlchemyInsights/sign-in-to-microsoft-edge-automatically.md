---
title: Automatické přihlášení k Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050687"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatické přihlášení k Microsoft Edge

Microsoft Edge používá výchozí účet operačního systému k automatickému přihlášení uživatele podle konfigurace zařízení uživatele. 

Scénáře jednotlivých typů konfigurace zařízení a procesu přihlášení závislých uživatelů jsou popsané níže:

- **Zařízení je hybridní/AAD-J:** Tato možnost je dostupná v Windows 10, nižších úrovních Windows a odpovídajících serverových verzích. Uživatelé se automaticky přihlášeni pomocí svých Azure Active Directory (AD)účtů.
- **Zařízení je připojené k doméně:** Tato možnost je dostupná v Windows 10, nižších úrovních Windows a odpovídajících serverových verzích. Ve výchozím nastavení se uživatelé s účty domény nepřichytují automaticky. pokud chcete povolit automatické přihlašování, použijte zásadu **ConfigureOnPremisesAccountAutoSignIn.** Pokud chcete povolit automatické přihlašování pro uživatele s účty Azure AD, zvažte hybridní připojení k jejich zařízením.
- **Výchozí účet operačního** systému je účet Microsoft: Tato možnost je dostupná v systému Windows 10 RS3 (verze 1709, build 10.0.16299) a novějších verzích. Scénář se pravděpodobně nevyskytuje na podnikových zařízeních. Pokud je ale výchozím účtem operačního systému účet Microsoft, Microsoft Edge se automaticky přihlásí k uživateli pomocí účtu Microsoft.
 
 
