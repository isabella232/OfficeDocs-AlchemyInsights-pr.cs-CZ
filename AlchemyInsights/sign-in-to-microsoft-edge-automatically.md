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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676966"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatické přihlášení k Microsoft Edge

Microsoft Edge používá výchozí účet operačního systému k automatickému přihlášení uživatele podle toho, jak je nastavené zařízení uživatele. 

Tady jsou popsané scénáře jednotlivých typů konfigurací zařízení a jeho proces přihlašování závislým uživatelem:

1. **Zařízení je hybridní/AAD-J**: Tato možnost je k dispozici ve Windows 10, Windows pro nižší verzi a v odpovídajících serverových verzích. Uživatelé se automaticky přihlásí pomocí svých účtů služby Azure Active Directory (AD).
2. **Zařízení je spojené s doménou**: Tato možnost je k dispozici ve Windows 10, Windows pro nižší úrovni a v odpovídajících serverových verzích. Ve výchozím nastavení nejsou uživatelé s účty domény automaticky přihlášeni. Pokud chcete povolit automatické přihlašování, použijte zásady **ConfigureOnPremisesAccountAutoSignIn** . Pokud chcete povolit automatické přihlašování pro uživatele s účty Azure AD, zvažte hybridní připojení svých zařízení.
3. **Výchozím účtem operačního systému je účet Microsoft**: Tato možnost je dostupná ve Windows 10 RS3 (verze 1709, Build 10.0.16299) a novější verze. U podnikových zařízení se nepravděpodobná situace. Pokud je ale výchozím účtem operačního systému účet Microsoft, Microsoft Edge ho automaticky přihlásí pomocí účtu Microsoft.
 
 
