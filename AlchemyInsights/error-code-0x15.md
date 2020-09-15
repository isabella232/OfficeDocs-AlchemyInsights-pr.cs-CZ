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
description: Pokud se při aktivaci Office 2013 na nasazení služby Vzdálená plocha (RDS) zobrazuje chyba, zvažte povolení funkce ADAL úpravou registru.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709180"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba při aktivaci Office 2013 na vzdálené ploše

Pokud se při aktivaci Office 2013 na nasazení služby Vzdálená plocha (RDS) zobrazuje chyba, zvažte povolení funkce ADAL úpravou registru.
  
|**Klíč registru**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |0,1  <br/> |

Další informace najdete v tématu [Povolení moderního ověřování pro Office 2013 na zařízeních s Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je ve výchozím nastavení aplikací Microsoft 365 pro podniky a Office 2016 povolen. Vzdálená plocha (RDS) se dřív jmenovala Terminálová služba.
  