---
title: PowerShell SharePointu Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770832"
---
# <a name="sharepoint-online-powershell"></a>PowerShell SharePointu Online

Pracujete s PowerShellem nebo skripty v SharePointu Online? Další informace najdete v následujících odkazech.
- [Začínáme s prostředím SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Připojení k SPO PowerShellu s vícefaktorového ověřováním (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Vzory a postupy služby SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahují knihovnu příkazů PowerShellu, která umožňuje provádět složité akce správy ke spo.

> [!NOTE]
> - Pokud máte problémy s připojením pomocí prostředí SPO Management Shell, ujistěte se, že jste aktualizovali nejnovější verzi, a zkuste [modul importovat znovu](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocí *modulu import – Microsoft. online. SharePoint. PowerShell* .
> - Pokud zkoušíte spustit skripty objektového modelu na straně klienta, budete muset mít na místním počítači nainstalovanou [sadu SDK součástí klienta SharePointu Online](https://www.microsoft.com/download/details.aspx?id=42038) .
> - Pokud máte problémy se spouštěním skriptů z PowerShellu, můžete zvážit, že se PowerShell spouští jako správce a změní se [zásady spuštění](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).