---
title: Práce s ID pravidla aplikace VPP pro iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083007"
---
# <a name="working-with-ios-vpp-applications"></a>Práce s aplikacemi VPP pro iOS

Přečtěte si článek Jak spravovat aplikace pro iOS zakoupené prostřednictvím [multilicenčního](https://docs.microsoft.com/intune/vpp-apps-ios) programu s aplikací Microsoft Intune, kde se dozvíte o funkcích, omezeních a krocích, jak v aplikaci Apple Volume Purchase Program používat program pro multilicenční nákup a podporu pro Microsoft Intune.
  
 **Běžné problémy:** "Uživatelům jsem přiřadil aplikaci VPP pro iOS, ale instalace se nezdařila."
  
- K tomu může dojít v případě, že se jeden token VPP používá napříč několika poskytovateli správy mobilních zařízení. Tokeny VPP od Společnosti Apple se smí používat jenom u jednoho poskytovatele. Pokud jste použili token VPP s více zprostředkovateli, musíte ho znovu nahrát do Intune.

- Instalace může také selhat, pokud celkový počet instalací překročí počet licencí. Pokud chcete zobrazit sestavu využití licencí, přejděte na stránku Licence aplikací **Intune Mobile** \>  Apps. Informace o tom, jak uvolnit užíné licence, najdete [v tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
