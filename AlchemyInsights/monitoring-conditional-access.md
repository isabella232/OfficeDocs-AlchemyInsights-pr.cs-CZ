---
title: Monitorování podmíněného přístupu
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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708667"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorování podmíněného přístupu pro Exchange

Pokud uživatelé, na které podmíněný přístup zacílete, nesplňuje požadavky organizace na přístup, dostanou e-mail s oznámením. Jako řešení doporučujeme jedno nebo více z následujících řešení:

- Pokud by už zařízení mělo být zaregistrované, poraďte uživateli, aby přecoval aplikaci Portál společnosti a ověřil, jestli se na portálu společnosti objeví. Pokud ne, měl by uživatel zařízení zaregistrovat.
- Na portálu Azure Portal přejděte na Intune > dodržování předpisů zařízením. V části Monitorovat klikněte na Dodržování předpisů zařízením. Prohlédněte si sestavu o dodržování předpisů zařízením a ověřte, jestli je zařízení uživatele označené jako zařízení dodržující předpisy.
- Na portálu Azure Portal přejděte na Intune > dodržování předpisů zařízením. V části Spravovat klikněte na Zásady. V seznamu zásad dodržování předpisů ověřte, jestli má zařízení uživatele přiřazený profil. Pokud není žádný profil přiřazený, nebude moct Intune ověřit stav dodržování předpisů zařízení.
- Upravte přiřazení podmíněného přístupu uživatele.

1. Na portálu Azure Portal přejděte na Zásady  >  **podmíněného přístupu**  >  Intune.
2. V seznamu vyberte zásadu.
3. Klikněte na Uživatelé a skupiny.
4. Pokud chcete určité zásady na někoho zacílit, přidejte ho do seznamu Zahrnout. Pokud chcete zajistit, aby byla osoba ze zásad vynechána, přidejte ji do seznamu Vyloučit.

Užitečné odkazy:

[Přehled dodržování předpisů zařízením](https://docs.microsoft.com/intune/device-compliance-get-started)

[Řešení potíží s CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zásady pro řešení potíží](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorování dodržování předpisů zařízením Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Poznámka: Tento postup je užitečný jenom při řešení potíží s podmíněným přístupem funkce Azure Active Directory. Taky je možné umístit zařízení do karantény, které zablokuje přístup k e-mailu pomocí zásad Exchange. Další informace o správě zařízení exchange najdete [tady]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)
