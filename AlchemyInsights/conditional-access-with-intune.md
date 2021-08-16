---
title: Podmíněný přístup pomocí Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069705"
---
# <a name="conditional-access-with-intune"></a>Podmíněný přístup pomocí Intune

Použití  **podmíněného přístupu v**  Intune vyžaduje 3 kroky:

- Vytvořte zásady **dodržování předpisů** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a definujte nastavení, která musí být splněna, než bude zařízení považované za kompatibilní. Zařízení musí mít například špendlík s aspoň 6 číslicemi, aby bylo považováno za vyhovující.
- Vytvořte zásadu **podmíněného přístupu,**  která definuje, jaké prostředky jsou chráněné a jaké podmínky je potřeba splnit pro přístup k teým prostředkům.  [Před přístupem](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  k podnikovému e-mailu musí být například zařízení kompatibilní.
- **Zajistěte, aby zásady dodržování** předpisů i zásady **podmíněného** přístupu byly zaměřené na požadované skupiny uživatelů. To může vyžadovat vytvoření konkrétních skupin uživatelů v Azure Active Directory.

**Užitečné odkazy:**

[Přehled dodržování předpisů pro zařízení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Poradce při potížích s certifikační autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Poradce při potížích se zásadou](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Pokud chcete chránit e-mail (Exchange online) před přístupem zařízení, která nejsou v režimu nedokonalých služeb, je nutné dodržovat oba dokumenty:

1. [Ochrana přístupu k e-mailu ze zařízení pomocí EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrana přístupu k e-mailu před zařízeními pomocí moderních ověřovacích klientů, jako je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)