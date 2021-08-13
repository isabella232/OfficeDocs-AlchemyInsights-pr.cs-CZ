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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975094"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorování podmíněného přístupu pro Exchange

Uživatelé s podmíněným přístupem dostanou e-mail s oznámením, pokud nesplňuje požadavky vaší organizace na přístup. K vyřešení doporučujeme jedno nebo více z následujících řešení:

- Pokud se předpokládá, že je zařízení zaregistrované, doporučíte uživateli, aby šel do aplikace Portál společnosti a ověřil, že se zobrazuje v Portál společnosti. Pokud ne, měl by si uživatel zařízení zaregistrovat.
- Na portálu Azure Portal přejděte na Intune > zařízení. V části Monitor klikněte na Dodržování předpisů pro zařízení. Zobrazte si zprávu o dodržování předpisů zařízení a ověřte, že je zařízení uživatele označené jako kompatibilní.
- Na portálu Azure Portal přejděte na Intune > zařízení. V části Spravovat klikněte na Zásady. V seznamu zásad dodržování předpisů ověřte, jestli je profil přiřazený k zařízení vašeho uživatele. Pokud není přiřazen žádný profil, Intune nebude moct potvrdit stav dodržování předpisů zařízení.
- Upravte přiřazení podmíněného přístupu uživatele.

1. Na portálu Azure Portal přejděte na **Zásady**  >  **podmíněného přístupu Intune**  >  .
2. Vyberte zásadu ze seznamu.
3. Klikněte na Uživatelé a skupiny.
4. Pokud chcete na někoho zacílit určitou zásadu, přidejte je do seznamu Zahrnout. Pokud chcete zajistit, aby byla osoba ze zásad vynechána, přidejte ji do seznamu Vyloučit.

Užitečné odkazy:

[Přehled dodržování předpisů pro zařízení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Poradce při potížích s certifikační autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Poradce při potížích se zásadou](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorování dodržování předpisů zařízení Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Poznámka: Tyto kroky jsou užitečné jenom při řešení potíží Azure Active Directory podmíněného přístupu. Je také možné umístit zařízení do karantény, které blokuje přístup k e-mailu pomocí Exchange zásad. Další informace o Exchange zařízení najdete [tady]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
