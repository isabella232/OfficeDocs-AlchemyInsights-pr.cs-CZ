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
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069237"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell a zastaralé základní ověřování

Nejnovější informace o tom, jak se připojit k PowerShellu pro Exchange Online bez použití základního ověřování, najdete [tady](https://aka.ms/exops-docs). Modul PowerShell V2 nepoužívá základní ověřování.

Mějte prosím na paměti, že základní ověřování musí být na klientském počítači nadále povolené.
Nový modul PowerShell V2 používá k navázání připojení u všech rutin V2 založených na rozhraní REST moderní ověřování. Kromě rutin V2 vám také umožňuje přístup ke starším rutinám vzdáleného PowerShellu (RPS), které vyžadují navázání relace vzdáleného PowerShellu. Navázání relace RPS na počítači s Windows vyžaduje, aby bylo na klientském počítači povolené ověřování WinRM BasicAuth, i když modul k ověření služby používá mechanismus moderního ověřování. K přenosu tokenů moderního ověřování se používá kanál základního ověřování WinRM. Pokud je na klientském počítači základní ověřování WinRM zakázané, budou nové rutiny V2 dál fungovat (ale ne starší rutiny RPS).
