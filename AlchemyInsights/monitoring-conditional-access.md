---
title: Sledování podmíněného přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366421"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Sledování podmíněného přístupu pro Exchange

Uživatelé s podmíněným přístupem budou dostávat e-mailové zprávy, pokud nesplňují požadavky na přístup vaší organizace. Chcete-li vyřešit problém, doporučujeme jedno nebo více následujících řešení:

- Pokud se předpokládá, že je zařízení zaregistrované, poraďte se s tím, že přejde do aplikace Portál společnosti a ověří, že se zobrazí na portálu společnosti. Pokud to nepomůže, uživatel by měl zařízení zaregistrovat.
- Na Azure Portal přejděte na Intune > dodržování předpisů zařízení. V části Monitor klikněte na položku dodržování předpisů. Zobrazte sestavu dodržování předpisů zařízení a ověřte, že zařízení uživatele je označené jako kompatibilní.
- Na Azure Portal přejděte na Intune > dodržování předpisů zařízení. V části Spravovat klikněte na zásady. V seznamu zásad dodržování předpisů ověřte, zda je k zařízení uživatele přiřazen profil. Pokud není přiřazen žádný profil, nebude moci Intune potvrdit jeho stav.
- Upravte přiřazení podmíněného přístupu uživatele.

1. V Azure Portal **přejděte na**  >  **zásady podmíněného přístupu**  >  **Policies**.
2. V seznamu vyberte zásadu.
3. Klikněte na uživatelé a skupiny.
4. Chcete-li určit určitou zásadu, přidejte ji do seznamu zahrnutí. Chcete-li zajistit, aby některá osoba byla ze zásady vynechána, přidejte ji do seznamu vyloučení.

Užitečné odkazy:

[Přehled dodržování předpisů zařízení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Poradce při potížích](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zásady řešení potíží](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorování dodržování předpisů zařízení](https://docs.microsoft.com/intune/compliance-policy-monitor)

Poznámka: Tento postup je užitečný jenom při odstraňování potíží s podmíněným přístupem Azure Active Directory. Je taky možné zablokovat zařízení blokující přístup k e-mailu pomocí zásad Exchange. Další informace o správě zařízení Exchange najdete [tady](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
