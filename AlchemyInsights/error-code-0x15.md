---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Pokud se při aktivaci systému Office 2013 v nasazeních služby Vzdálená plocha (RDS) zobrazí chybová zpráva, zvažte povolení funkce ADAL úpravou registru.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100755"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba při aktivaci Office 2013 ve Vzdálené ploše

Pokud se při aktivaci systému Office 2013 v nasazeních služby Vzdálená plocha (RDS) zobrazí chybová zpráva, zvažte povolení funkce ADAL úpravou registru.
  
|**Klíč registru**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Další informace najdete v tématu [Povolení moderního ověřování pro Office 2013 na Windows zařízeních.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  Funkce ADAL je ve výchozím nastavení v Microsoft 365 Apps pro velké organizace a Office 2016 povolená. Vzdálená plocha (RDS) se dříve jmenovala Terminálová služba.
  