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
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704779"
---
# <a name="conditional-access-with-intune"></a>Podmíněný přístup pomocí Intune

Použití  **podmíněného přístupu**  v Intune vyžaduje 3 kroky:

- Vytvořte zásady  **dodržování předpisů** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)definující nastavení, která musí být splněná, aby bylo zařízení považované za zařízení dodržující předpisy. Aby bylo zařízení považované za zařízení dodržující předpisy, musí mít například kód PIN aspoň 6 číslic.
- Vytvořte zásady **podmíněného přístupu,**  které definují, které prostředky jsou chráněné a jaké podmínky musí být pro přístup k zdrojům splněné.  [Aby mělo například zařízení](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  přístup k podnikovému e-mailu, musí být v souladu s předpisy.
- **Zajistěte, aby zásady dodržování** předpisů a zásady **podmíněného** přístupu byly cílené na požadované skupiny uživatelů. To může vyžadovat vytvoření konkrétních skupin uživatelů v Azure Active Directory.

**Užitečné odkazy:**

[Přehled dodržování předpisů zařízením](https://docs.microsoft.com/intune/device-compliance-get-started)

[Řešení potíží s CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zásady pro řešení potíží](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Pokud chcete e-mail (Exchange Online) chránit před přístupem zařízení, která nejsou s tím, jak mají být, musí následovat oba dokumenty:

1. [Ochrana přístupu k e-mailu ze zařízení pomocí EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrana přístupu k e-mailu ze zařízení pomocí moderních ověřovacích klientů, jako je outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)