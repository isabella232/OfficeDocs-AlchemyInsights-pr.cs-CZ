---
title: Chyba licencování služby Endpoint DLP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564417"
---
# <a name="endpoint-dlp-licensing-error"></a>Chyba licencování služby Endpoint DLP

Při pokusu o nastavení ochrany před únikem koncových bodů se zobrazí následující chybová zpráva:

`Your organization is missing the licenses required to manage these devices`.

Ujistěte se, že máte jedno z následujících předplatných nebo doplňků:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Dodržování předpisů v Microsoft 365 E5
- Dodržování předpisů v Microsoft 365 a5
- Microsoft 365 E5 Information Protection a vládnutí
- Microsoft 365 a5 – ochrana informací a vládnutí

> [!NOTE]
> Tento postup nefunguje pro kombinace licencí, jako jsou: Win E5 + O365 E5 + EMS E5. K nastavení této funkce potřebujete licenci Pure M365 E5.

Další informace o licencování [koncových](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management) bodů pro ochranu koncového bodu
