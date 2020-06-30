---
title: Podmíněný přístup s Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931423"
---
# <a name="conditional-access-with-intune"></a>Podmíněný přístup s Intune

Použití **podmíněného přístupu** s Intune vyžaduje 3 kroky:

- Vytvořte **zásady dodržování předpisů** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a definujte nastavení, která musí být splněna, aby bylo zařízení považováno za vyhovující. Zařízení musí mít například pin alespoň 6 číslic, aby bylo považováno za vyhovující.
- Vytvořte **zásady podmíněného přístupu,** které definují, jaké prostředky jsou chráněny a jaké podmínky je třeba splnit pro přístup k těmto prostředkům.  Zařízení musí být [například](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) kompatibilní před přístupem k podnikovému e-mailu.
- Ujistěte se, **že zásady dodržování předpisů** a **zásady podmíněného přístupu** jsou zaměřeny na požadované skupiny uživatelů. To může vyžadovat vytvoření konkrétních skupin uživatelů ve službě Azure Active Directory.

**Užitečné odkazy:**

[Přehled dodržování předpisů pro zařízení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Poradce při potížích s certifikační autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zásady řešení potíží](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Chcete-li chránit e-mail (Exchange online) před přístupem nekompatibilních zařízení, je třeba dodržovat oba dokumenty:

1. [Ochrana přístupu k e-mailu ze zařízení pomocí služby EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrana přístupu k e-mailu ze zařízení pomocí moderních klientů pro ověřování, jako je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)