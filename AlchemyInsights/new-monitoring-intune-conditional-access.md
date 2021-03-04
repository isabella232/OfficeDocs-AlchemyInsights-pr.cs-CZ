---
title: Sledování podmíněného přístupu Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427180"
---
# <a name="monitor-intune-conditional-access"></a>Sledování podmíněného přístupu Intune

Pokud uživatelé, na které podmíněný přístup zacílete, nesplňuje požadavky organizace na přístup, dostanou e-mail s oznámením. Jako řešení doporučujeme jedno nebo více z následujících řešení:

1. Pokud by už zařízení mělo být zaregistrované, poraďte uživateli, aby přecoval aplikaci Portál společnosti a ověřil, jestli se na portálu společnosti objeví. V tom případě musí uživatel zařízení zaregistrovat.
1. Na portálu Azure Portal přejděte na Dodržování **předpisů**  >  **zařízením** Intune. 
1. Pokud chcete zobrazit sestavu o dodržování předpisů zařízením a ověřit, jestli je zařízení uživatele označené jako zařízení dodržující předpisy, klikněte v části **Monitor** na **Dodržování předpisů zařízením.**
1. Na portálu Azure Portal přejděte na Dodržování **předpisů**  >  **zařízením** Intune. V **části Spravovat klikněte** na **Zásady.** V seznamu zásad dodržování předpisů ověřte, jestli má zařízení uživatele přiřazený profil. Pokud není žádný profil přiřazený, nebude moct Intune ověřit stav dodržování předpisů zařízení.
1. Upravte přiřazení podmíněného přístupu uživatele.
1. Na portálu Azure Portal přejděte na Zásady podmíněného přístupu **Intune,** vyberte zásadu ze seznamu a klikněte na  >    >  Uživatelé a **skupiny.**
1. Pokud chcete určité zásady na někoho zacílit, přidejte ho do **seznamu Zahrnout.** Pokud chcete zajistit, aby byla osoba ze zásad vynechána, přidejte ji do **seznamu Vyloučit.**

**Užitečné odkazy:**

- [Přehled dodržování předpisů zařízením](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Řešení potíží s CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Zásady pro řešení potíží](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorování dodržování předpisů zařízením Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Tyto kroky jsou užitečné jenom při řešení potíží s podmíněným přístupem funkce Azure Active Directory. Taky je možné umístit zařízení do karantény, které zablokuje přístup k e-mailu pomocí zásad Exchange. Další informace o správě zařízení Exchange najdete [**tady.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
