---
title: Podmíněný přístup s Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807652"
---
# <a name="conditional-access-with-intune"></a>Podmíněný přístup s Intune

Použití  **podmíněného přístupu**  s Intune vyžaduje 3 kroky:

- Vytvořením  **zásad dodržování předpisů**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) definujte nastavení, která musí být splněná, než se zařízení považuje za kompatibilní. Například zařízení musí mít PIN kód alespoň 6 číslic, než se považuje za vyhovující.
- Vytvořte **zásadu podmíněného přístupu**  definující prostředky, které se chrání, a jaké podmínky je třeba pro přístup k těmto prostředkům splnit.  Před [přístupem do](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) firemních e-mailů musí být zařízení kompatibilní.
- Zajistěte, aby **zásady dodržování předpisů**  a  **zásady podmíněného přístupu**  byly cílené na požadované skupiny uživatelů. To by mohlo vyžadovat vytvoření určitých skupin uživatelů v Azure Active Directory.

**Užitečné odkazy:**

[Přehled dodržování předpisů zařízení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Poradce při potížích](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zásady řešení potíží](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Chcete-li chránit E-mail (Exchange Online) z Accessu neodpovídajícími zařízeními, musí být dodržovány oba dokumenty:

1. [Ochrana přístupu k e-mailu ze zařízení pomocí EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrana e-mailových zpráv ze zařízení pomocí moderních klientů ověřování, jako je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)