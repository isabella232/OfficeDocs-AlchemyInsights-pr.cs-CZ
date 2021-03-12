---
title: Použití podmíněného přístupu v Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744542"
---
# <a name="using-conditional-access-with-intune"></a>Použití podmíněného přístupu v Intune

Použití podmíněného přístupu v Intune vyžaduje 3 kroky:

- [Vytvořte zásady dodržování předpisů a definujte nastavení, která musí být splněna, než bude zařízení považované za kompatibilní. Zařízení musí mít například špendlík s aspoň 6 číslicemi, aby bylo považováno za vyhovující.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Vytvořte zásadu podmíněného přístupu, která definuje, jaké prostředky jsou chráněné a jaké podmínky je potřeba splnit pro přístup k teým prostředkům. Před přístupem k podnikovému e-mailu musí být například zařízení kompatibilní.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Zajistěte, aby zásady dodržování předpisů i zásady podmíněného přístupu byly zaměřené na požadované skupiny uživatelů. To může vyžadovat vytvoření konkrétních skupin uživatelů v Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Další informace...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
