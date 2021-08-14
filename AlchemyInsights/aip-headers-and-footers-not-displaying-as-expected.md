---
title: 'AIP: Záhlaví a zápatí se nezobrazují podle očekávání'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: e3a0e5caccba87ddd8e4c786b5c8918494e709b6f4d5d60e7c31215a60b1d5d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951774"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: Záhlaví a zápatí se nezobrazují podle očekávání

Pokud máte problémy s vizuálními značkami, které se nezobrazují podle očekávání, podívejte se na následující pokyny:

1. Zkontrolujte, jestli jste si prohlédli [Při použití vizuálních znacích](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Pokud Office popisků, zkontrolujte, kdy Office 365 a šifrování [obsahu.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)
3. Pokud chcete odebrat existující záhlaví nebo zápatí, zkontrolujte Odebrání záhlaví a zápatí z jiných řešení [pro označování](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).

Pokud k tomuto problému stále dochází, shromážděte protokoly klienta Azure Information Protection a připojte exportované protokoly k tomuto lístku.

**Export protokolů Azure Information Protection**

1. Otevřete dokument Office nebo vytvořte nový e-mail v Outlook.
2. Klikněte **na Zamknout/Citlivost**  >  **– nápověda a zpětná vazba.**
3. Klikněte **na Exportovat protokoly**.
4. Protokoly uložte do volby umístění a připojte je k této žádosti o službu.

Další informace najdete v těchto informacích:

- [Jak nakonfigurovat popisek pro vizuální označení pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Kontrola dokumentace k Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Požadavky na Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Úvodní kurz pro Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Stažení klienta Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
