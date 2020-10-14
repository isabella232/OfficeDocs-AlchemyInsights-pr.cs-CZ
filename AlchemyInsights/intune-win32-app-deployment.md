---
title: Nasazení aplikací Win32 v Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461757"
---
# <a name="intune-win32-app-deployment"></a>Nasazení aplikací Win32 v Intune

Microsoft Intune umožňuje aplikacím Win32, včetně nejenom se službou MSI a. EXE pro nasazení na zařízení s Windows 10. Použitý mechanismus nasazení vyžaduje, aby byla na cílovém zařízení přítomná rozšíření pro správu Intune. Editor IME bude automaticky nainstalován jako výsledek zaměření nasazení skriptu PowerShell nebo Win32 na zařízení.

Existují také systémy předpokladů, které musí být splněny, aby bylo možné nasadit aplikace Win32, které zahrnují:

- Podporované platformy: Windows 10 verze 1607 nebo novější (verze Enterprise, pro a vzdělávací organizace).
- Podporovaná architektura: x86 a x64
- Správa zařízení: připojení k AAD a automaticky zaregistrované (včetně připojení hybridní domény a automaticky zapsaných zásad skupiny).
- Formát balíčku aplikace:. **intunewin**  soubor připravený nástrojem pro [přípravu obsahu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Kladen
    - Maximální velikost: 8 GB.
    - Nepodporovaná architektura: paže.

Projděte si dokument "[Přidání, přiřazení a monitorování aplikace Win32 v Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)", kde najdete další informace o těchto krocích.

Podrobnosti o řešení potíží s nasazením aplikací v systému Windows, včetně aplikací Win32, najdete v následujících dokumentech.

- [Poradce při potížích s instalací aplikace](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Odstraňování potíží s aplikacemi Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)