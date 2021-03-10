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
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692697"
---
# <a name="using-conditional-access-with-intune"></a>Použití podmíněného přístupu v Intune

Použití podmíněného přístupu v Intune vyžaduje 3 kroky:

- [Vytvořte zásady dodržování předpisů definující nastavení, která musí být splněná, aby bylo zařízení považované za zařízení dodržující předpisy. Aby bylo zařízení považované za zařízení dodržující předpisy, musí mít například kód PIN aspoň 6 číslic.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Vytvořte zásady podmíněného přístupu, které definují, které prostředky jsou chráněné a jaké podmínky musí být pro přístup k zdrojům splněné. Aby mělo například zařízení přístup k podnikovému e-mailu, musí být v souladu s předpisy.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Zajistěte, aby zásady dodržování předpisů a zásady podmíněného přístupu byly cílené na požadované skupiny uživatelů. To může vyžadovat vytvoření konkrétních skupin uživatelů v Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Další informace...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
