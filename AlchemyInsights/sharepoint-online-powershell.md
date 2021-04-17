---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830575"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Pracujete s PowerShellem nebo skripty v SharePointu Online? Další informace najdete v následujících odkazech.
- [Začínáme s prostředím SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Připojení k prostředí SPO PowerShell pomocí vícefaktorového ověřování (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahuje knihovnu příkazů PowerShellu, které vám umožní provádět složité akce správy směrem ke službě SPO.

> [!NOTE]
> - Pokud máte problémy s připojením k prostředí pro správu spo, ujistěte se, že jste aktualizovali na nejnovější verzi, a zkuste modul znovu importovat pomocí importu modulu *Microsoft.Online.SharePoint.PowerShell.* [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)
> - Pokud se pokoušíte spustit skripty modelu objektu na straně klienta, budete muset mít na místním počítači nainstalovanou [sadu SHAREPOINT Online Client Components SDK.](https://www.microsoft.com/download/details.aspx?id=42038)
> - Pokud máte problémy se spouštěním skriptů z PowerShellu, můžete zvážit spuštění PowerShellu jako správce a změnu zásad [spuštění.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)