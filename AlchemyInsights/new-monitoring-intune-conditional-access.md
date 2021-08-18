---
title: Monitorování podmíněného přístupu k Intune
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
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327550"
---
# <a name="monitor-intune-conditional-access"></a>Monitorování podmíněného přístupu k Intune

Uživatelé s podmíněným přístupem dostanou e-mail s oznámením, pokud nesplňuje požadavky vaší organizace na přístup. K vyřešení doporučujeme jedno nebo více z následujících řešení:

1. Pokud se předpokládá, že je zařízení zaregistrované, doporučíte uživateli, aby šel do aplikace Portál společnosti a ověřil, že se zobrazuje v Portál společnosti. Pokud ne, musí si uživatel zařízení zaregistrovat.
1. Na portálu Azure Portal přejděte na **Dodržování předpisů zařízení Intune**  >  . 
1. Pokud chcete zobrazit zprávu o dodržování předpisů zařízení, abyste ověřili, že je zařízení uživatele označené jako kompatibilní, klikněte v části **Monitor** na **Shoda zařízení.**
1. Na portálu Azure Portal přejděte na **Dodržování předpisů zařízení Intune**  >  . V **části Manage (Spravovat)** klikněte na **Policies (Zásady).** V seznamu zásad dodržování předpisů ověřte, jestli je profil přiřazený k vašemu zařízení uživatele. Pokud není přiřazen žádný profil, Intune nebude moct potvrdit stav dodržování předpisů zařízení.
1. Upravte přiřazení podmíněného přístupu uživatele.
1. Na portálu Azure Portal přejděte na **Zásady podmíněného** přístupu Intune , vyberte zásadu ze seznamu  >    >  a klikněte na Uživatelé a **skupiny.**
1. Pokud chcete na někoho zacílit určitou zásadu, přidejte je do **seznamu Zahrnout**. Pokud chcete zajistit, aby byla osoba ze zásad vynechána, přidejte ji do **seznamu Vyloučit**.

**Užitečné odkazy:**

- [Přehled dodržování předpisů pro zařízení](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Poradce při potížích s certifikační autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Poradce při potížích se zásadou](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorování dodržování předpisů zařízení Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Poznámka:** Tyto kroky jsou užitečné jenom při řešení potíží Azure Active Directory podmíněného přístupu. Je také možné umístit zařízení do karantény, které blokuje přístup k e-mailu pomocí Exchange zásad. Další informace o Exchange zařízení najdete [**tady**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
