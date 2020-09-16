---
title: Intune profily Wi-Fi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696254"
---
# <a name="intune-wi-fi-profiles"></a>Intune profily Wi-Fi

Úspěšná implementace připojení Wi-Fi pro klienty MDM závisí na správně nasazeném profilu, který odráží požadavky podnikové infrastruktury Wi-Fi. Pokud chcete zkontrolovat příslušná nastavení pro klientské platformy, které zkoumáte, přečtěte si téma: 

[Přidání nastavení Wi-Fi pro zařízení s Androidem v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Přidání nastavení Wi-Fi pro podniková vyhrazená a plně spravovaná zařízení s Androidem v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Přidání nastavení Wi-Fi pro zařízení s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Přidání nastavení Wi-Fi pro Windows 10 a novější zařízení v Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Import nastavení Wi-Fi pro zařízení s Windows v Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Běžné problémy**

**Zavádím profil sítě Wi-Fi, který je závislý na nasazeném certifikátu zadaném v profilu sítě Wi-Fi. Konfigurační profily však zobrazují chybový stav.**

Zkontrolujte, že vaše zařízení certifikát obdržel.

1. V Intune přejděte na **všechna zařízení** a vyberte zařízení > **konfiguraci zařízení**.

2. Zkontrolujte, jestli jsou všechny očekávané profily uvedené a v úspěšném stavu.

3. Pokud máte v řetězci certifikátu zprostředkující certifikáty, ujistěte se, že jsou na zařízení s Androidem nasazené.

    Pokud chcete zkontrolovat stav certifikátu, přejděte na **konfigurační**  >  **profily**zařízení  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.

Pokud se vám pořád zobrazují chyby, podívejte se na postupy a oddíly řešení potíží. Další informace najdete v článku [o řešení potíží s profily certifikátů SCEP přes Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Nasadil (a) profil sítě Wi-Fi na zařízení. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k Wi-Fi.**

Úspěšný stav znamená, že v Intune se profil úspěšně nasadil jako nakonfigurovaný. Tato konfigurace ale nemusí odpovídat vašim požadavkům na síť nebo ověřování. Další podrobnosti o pokusu o připojení najdete v protokolech v tématu infrastruktura a ověřování (na řadiči přístupových bodů sítě Wi-Fi a serveru NPS nebo RADIUS). Možná budete muset pracovat s týmem infrastruktury sítě nebo s poskytovatelem Wi-Fi jiného výrobce, abyste mohli shromáždit a zkontrolovat protokoly.