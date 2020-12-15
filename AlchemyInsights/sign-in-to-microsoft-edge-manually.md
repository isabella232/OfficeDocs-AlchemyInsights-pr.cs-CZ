---
title: Přihlášení k Microsoft Edge ručně
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676971"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Přihlášení k Microsoft Edge ručně

Pokud se uživatel během prvního spuštění automaticky přihlásil, může se přihlásit pomocí nastavení prohlížeče nebo prostřednictvím informačního panelu identity. Pokud chcete spravovat přihlašování, použijte tyto zásady:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – zajistěte, aby uživatel měl vždy pracovní profil v Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – omezení přihlášení na sadu důvěryhodných účtů.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – zakažte přihlášení nebo vynuťte přihlášení uživatelů.

