---
title: Profily Wi-Fi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554856"
---
# <a name="intune-wi-fi-profiles"></a>Profily Wi-Fi Intune

Úspěšná implementace wi-fi připojení pro klienty MDM závisí na správně nasazeném profilu, který odráží požadavky podnikové infrastruktury Wi-Fi. Chcete-li zkontrolovat příslušná nastavení pro klientské platformy, které zkoumáte, naleznete v následujících tématech: 

[Přidání nastavení Wi-Fi pro zařízení se systémem Android v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Přidání nastavení Wi-Fi pro vyhrazená a plně spravovaná zařízení Android Enterprise v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Přidání nastavení Wi-Fi pro iOS a iPadOS zařízení v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Přidání nastavení Wi-Fi pro zařízení s Windows 10 a novějšími v Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Import nastavení Wi-Fi pro zařízení s Windows v Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Běžné problémy**

**Nasazuji profil Wi-Fi, který je závislý na nasazeném certifikátu určeném v profilu Wi-Fi. Konfigurační profily však zobrazují stav chyby.**

Zkontrolujte, zda zařízení obdrželo certifikát.

1. V Intune přejděte na **Všechna zařízení** a vyberte zařízení > **konfiguraci zařízení**.

2. Zkontrolujte, zda jsou uvedeny všechny očekávané profily a v úspěšném stavu.

3. Pokud máte v řetězu certifikátů zprostředkující certifikáty, ujistěte se, že jsou nasazené do zařízení s Androidem.

    Chcete-li zkontrolovat stav certifikátu, **přejděte**na profily konfigurace zařízení  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.

Pokud se chyby budou zobrazovat i nadále, přečtěte si části postupy a řešení potíží. Další informace najdete v [tématu Přehled řešení potíží s profily certifikátů SCEP pomocí Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Do zařízení jsem nasadil profil Wi-Fi. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k Wi-Fi.**

Úspěšný stav znamená, že Intune úspěšně nasadil profil tak, jak byl nakonfigurovaný. Tyto konfigurace však nemusí odpovídat požadavkům na síť nebo ověřování. Další podrobnosti o pokusu o připojení naleznete v protokolech v infrastruktuře a službě ověřování (na řadiči přístupových bodů Wi-Fi a serveru NPS/Radius). Možná budete muset spolupracovat s týmem síťové infrastruktury nebo s externím dodavatelem Wi-Fi, abyste shromáždili a zkontrolovali protokoly.