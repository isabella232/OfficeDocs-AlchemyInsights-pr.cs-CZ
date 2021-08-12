---
title: Problémy související s VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970972"
---
# <a name="vpn-related-issues"></a>Problémy související s VPN

Úspěšná implementace připojení VPN pro klienty MDM závisí na nasazeném profilu, který správně odpovídá požadavkům infrastruktury VPN. Příslušná nastavení pro klientské platformy, které prošetřujeme, najdete v těchto tématu: 

[Windows 10 a Windows holografického zařízení pro přidání připojení VPN pomocí Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Přidání nastavení VPN na zařízeních s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Nastavení zařízení s Androidem pro konfiguraci VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Přidání nastavení VPN na zařízeních s macOS v Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Pokud váš profil VPN používá ověřování založené na certifikátech, ujistěte se, že jsou profily kořenových certifikátů a klientských ověřovacích certifikátů propojené s profilem VPN úspěšně nasazené.

**Běžné problémy**

**Na zařízení jsem nasadil(a) profil VPN. Intune ukazuje, že byla úspěšná, ale zařízení se k VPN ne připojuje.**

Úspěšný stav znamená, že Intune úspěšně nasadila profil tak, jak je nakonfigurovaný. Tyto konfigurace ale nemusí odpovídat požadavkům na síť nebo ověřování. Další podrobnosti o pokusu o připojení najdete v protokolech infrastruktury a ověřovací služba (na serveru VPN a serveru NPS/Radius). Možná budete muset spolupracovat se svým týmem síťové infrastruktury nebo s dodavatelem VPN od jiného výrobce, abyste mohli shromažďovat a zkontrolovat protokoly.

**Když nakonfiguruji vlastní VPN pro iOS, funkce VPN pro každou aplikaci není dostupná.**

Vpn pro jednotlivé aplikace pro zařízení s iOS v Intune je v současné době k dispozici pro konkrétní seznam poskytovatelů a partnerů, kteří musí také splňovat požadavky na certifikát před konfigurací VPN pro jednotlivé aplikace. Další informace najdete v článku Nastavení virtuální privátní sítě (VPN) pro zařízení [s iOS/iPadOS](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)v Intune pro každou aplikaci. 

Další informace o všech typech připojení VPN v Intune najdete v tématu Vytvoření profilů VPN pro připojení k [serverům VPN v Intune.](https://docs.microsoft.com/intune/vpn-settings-configure)  

**Vpn na vyžádání v iOSu se nespouštěla při přístupu k nakonfigurované doméně.**

Pokud chcete otestovat automatická nastavení VPN, nastavte následující hodnoty:

Chci udělat toto: **Vyhodnocení každého pokusu o připojení** 

Zvolte, jestli se chcete připojit: **Připojení v případě potřeby**

Při přístupu uživatelů k těmto doménám: **název** *cílové domény*

Pokud výše uvedená konfigurace není úspěšná, přidejte následující prvek:

Pokud není tato adresa URL nedostupná, vynučte připojení VPN: **BADURL**