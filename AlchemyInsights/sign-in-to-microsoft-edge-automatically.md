---
title: Automatické přihlášení k Microsoft Edgi
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398722"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatické přihlášení k Microsoft Edgi

Microsoft Edge používá výchozí účet operačního systému k automatickému přihlášení uživatele podle toho, jak je nakonfigurované zařízení uživatele. 

Scénáře jednotlivých typů konfigurace zařízení a procesu přihlášení závislých uživatelů jsou popsané níže:

- **Zařízení je hybridní/AAD-J:** Tato možnost je dostupná ve Windows 10, na nižší úrovni Windows a odpovídajících serverových verzích. Uživatelé se automaticky přihlášeni pomocí svých účtů Azure Active Directory (AD).
- **Zařízení je připojené k doméně:** Tato možnost je dostupná ve Windows 10, ve Windows nižší úrovni a odpovídajících serverových verzích. Ve výchozím nastavení se uživatelé s účty domény nepřichytují automaticky. pokud chcete povolit automatické přihlašování, použijte zásadu **ConfigureOnPremisesAccountAutoSignIn.** Pokud chcete povolit automatické přihlašování pro uživatele s účty Azure AD, zvažte hybridní připojení k jejich zařízením.
- **Výchozí účet operačního** systému je účet Microsoft: Tato možnost je dostupná ve Windows 10 RS3 (verze 1709, build 10.0.16299) a novějších verzích. Scénář se pravděpodobně nevyskytuje na podnikových zařízeních. Pokud je ale výchozím účtem operačního systému účet Microsoft, Microsoft Edge se automaticky přihlásí k uživateli pomocí účtu Microsoft.
 
 
