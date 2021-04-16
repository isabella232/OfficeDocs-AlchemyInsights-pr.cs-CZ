---
title: Exchange PowerShell a zastaralé základní ověřování
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813465"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell a zastaralé základní ověřování

Nejnovější informace o tom, jak se připojit k PowerShellu pro Exchange Online bez použití základního ověřování, najdete [tady](https://aka.ms/exops-docs). Modul PowerShell V2 nepoužívá základní ověřování.

Mějte prosím na paměti, že základní ověřování musí být na klientském počítači nadále povolené.
Nový modul PowerShell V2 používá k navázání připojení u všech rutin V2 založených na rozhraní REST moderní ověřování. Kromě rutin V2 vám také umožňuje přístup ke starším rutinám vzdáleného PowerShellu (RPS), které vyžadují navázání relace vzdáleného PowerShellu. Navázání relace RPS na počítači s Windows vyžaduje, aby bylo na klientském počítači povolené ověřování WinRM BasicAuth, i když modul k ověření služby používá mechanismus moderního ověřování. K přenosu tokenů moderního ověřování se používá kanál základního ověřování WinRM. Pokud je na klientském počítači základní ověřování WinRM zakázané, budou nové rutiny V2 dál fungovat (ale ne starší rutiny RPS).
