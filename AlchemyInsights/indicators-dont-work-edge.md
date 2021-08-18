---
title: Indikátory nefungují v prohlížeči Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326254"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikátory nefungují v prohlížeči Edge

Po vytvoření indikátoru ho Edge (Smartscreen) nebude ctít. Další informace najdete v tématu Vytvoření indikátorů pro IP adresy a [adresy URL/domény](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Krok 1: Ujistěte se, že jste na následujícím kroku:

- Ověřte, jestli je indikátor správný (žádné překlepy v IP/URL, správná akce, správné skupiny RBAC).
- Počkejte minimálně 2 hodiny po vytvoření indikátoru, aby se zohlednila jakákoli možná latence.
- Ujistěte se, že jsou systém(y) v programu Microsoft Defender for Endpoint.
- Ověřte, jestli systém(y) může komunikovat s cloudem.
- Ověřte, jestli je smartscreen povolený a dosažitelný, a to tak, že se dostanete na [testovací web.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Krok 2: Řešení potenciálního problému

- Ujistěte se, že klient splňuje požadavky. Podrobnosti najdete v tématu Vytvoření indikátorů pro IP adresy a [adresy URL/domény](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Ujistěte se, že používáte nejnovější verzi prohlížeče Edge. Informace o nejnovější verzi najdete v tématu Zjistěte, kterou [Microsoft Edge máte](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Restartujte prohlížeč Edge.
- Přejděte na web, pro který máte nastavit indikátor. Pokud se web nezobrazuje očekávaným způsobem, pokračujte krokem 3. 

## <a name="step-3-collect-data"></a>Krok 3: Shromažďování dat

- Shromažďování **diagnostických dat MDEClientAnalyzer** Pokyny najdete v tématu Problémy s zařízeními pro připojení k [Microsoft Defenderu pro koncový bod](issues-with-onboarding-machines.md).
- Pokud máte s instalací a shromažďováním stop fiddlerů problém, podívejte se na [stránku Telerik Fiddler](http://www.telerik.com/fiddler).
- Pokud upřednostňujete pokyny od podpory Microsoftu, vyberte níže ikonu Podpora a otevřete tak případ podpory.
