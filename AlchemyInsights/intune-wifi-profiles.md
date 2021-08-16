---
title: Profily Wi-Fi Intune
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
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028213"
---
# <a name="intune-wi-fi-profiles"></a>Profily Wi-Fi Intune

Úspěšná implementace Wi-Fi pro klienty MDM závisí na správně nasazené profil, který odpovídá požadavkům podnikové Wi-Fi infrastruktury. Pokud chcete zkontrolovat příslušná nastavení pro klientské platformy, které prošetřujeme, podívejte se na následující informace: 

[Přidání Wi-Fi pro zařízení s Androidem v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Přidání Wi-Fi nastavení pro zařízení s Androidem Enterprise vyhrazená a plně spravovaná zařízení v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Přidání Wi-Fi pro zařízení s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Přidání Wi-Fi nastavení pro Windows 10 a novější zařízení v Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Import Wi-Fi nastavení pro Windows zařízení v Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Běžné problémy**

**Nasazuji profil Wi-Fi, který je závislý na nasazené certifikátu zadaném v Wi-Fi profilu. V konfiguračních profilech se ale zobrazuje chybový stav.**

Zkontrolujte, že vaše zařízení certifikát obdrželo.

1. V Intune přejděte na **Všechna zařízení** a vyberte zařízení, > **zařízení**.

2. Zkontrolujte, že jsou všechny očekávané profily uvedené a v úspěšném stavu.

3. Pokud máte v řetězu certifikátů zprostředkující certifikáty pro androidový profil, ujistěte se, že jsou nasazené na zařízeních s Androidem.

    Pokud chcete zkontrolovat stav certifikátu, přejděte na **Profily konfigurace** zařízení Android  >    >  **intermediate CA**  >  **Properties**  >  **Trusted Certificate**.

Pokud chyby vidíte i nadále, podívejte se na postupy a oddíly pro řešení potíží. Další informace najdete v tématu [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Nasadil(a) jsem Wi-Fi profil na zařízení. Intune ukazuje, že byla úspěšná, ale zařízení se k Wi-Fi ne připojuje.**

Úspěšný stav znamená, že Intune úspěšně nasadila profil tak, jak je nakonfigurovaný. Tyto konfigurace ale nemusí odpovídat požadavkům na síť nebo ověřování. Další podrobnosti o pokusu o připojení najdete v protokolech v infrastruktuře a ověřovací služba (na řadiči accessových bodů Wi-Fi serveru NPS/Radius). Možná budete muset spolupracovat se svým týmem síťové infrastruktury nebo s dodavatelem třetí Wi-Fi, abyste shromáždili a prošli protokoly.