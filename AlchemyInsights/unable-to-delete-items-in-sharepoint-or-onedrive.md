---
title: Položky v aplikaci SharePoint nebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038510"
---
# <a name="unable-to-delete-items"></a>Položky se nedaří odstranit.

- Zásady uchovávání informací to mohou způsobit, musíte buď zakázat nebo vyloučit příslušné blokování, které způsobuje tento problém. Po odebrání zásady uchovávání informací nebo blokování může trvat až 24 hodin, než se změna projeví. Ujistěte se, že u položky [není](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) nastavená zásada uchovávání informací.

- Web možná překročil limit úložiště, zvýšil [kvótu webu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstranil položku.

- Zkontrolujte, že položka není [rezervována jinému](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) uživateli.

- Správci můžou také [používat SharePoint vzory](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) a postupy (PnP), které obsahují knihovnu příkazů PowerShellu, které umožňují provádět složité akce správy, jako je vynucení odstranění neústupných položek.
- [Odebrání souboru PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odebrání složky PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odebrání položky seznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odebrání seznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odebrat pole PNP (sloupec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)