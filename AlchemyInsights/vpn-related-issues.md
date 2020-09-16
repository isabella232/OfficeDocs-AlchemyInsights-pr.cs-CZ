---
title: Problémy související se sítí VPN
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
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726084"
---
# <a name="vpn-related-issues"></a>Problémy související se sítí VPN

Úspěšná implementace připojení VPN pro klienty MDM závisí na nasazeném profilu, který správně odráží požadavky infrastruktury VPN. Příslušné možnosti pro klientské platformy, které zkoumáte, najdete v tématu: 

[Nastavení zařízení s Windows 10 a celoplošným Holografickím přidání připojení VPN pomocí Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Přidání nastavení sítě VPN pro zařízení s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Nastavení zařízení s Androidem pro konfiguraci VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Přidání nastavení sítě VPN na zařízení macOS v Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Pokud váš profil sítě VPN používá ověřování založené na certifikátech, ujistěte se, že jsou profily certifikátů kořenového certifikátu a ověřování klientů propojené se svým profilem VPN úspěšně nasazené.

**Běžné problémy**

**Na zařízení je nasazený profil sítě VPN. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k síti VPN.**

Úspěšný stav znamená, že v Intune se profil úspěšně nasadil jako nakonfigurovaný. Tato konfigurace ale nemusí odpovídat vašim požadavkům na síť nebo ověřování. Další podrobnosti o pokusu o připojení najdete v protokolech v tématu infrastruktura a ověřování (na serveru VPN a serveru NPS/RADIUS). Pro shromáždění a kontrolu protokolů může být potřeba pracovat se svým týmem infrastruktury sítě nebo s dodavatelem VPN jiného výrobce.

**Když nakonfigurujem vlastní připojení VPN pro iOS, funkce VPN pro jednotlivé aplikace není dostupná.**

Připojení VPN pro zařízení s iOS v Intune je v současné době dostupné pro konkrétní seznam poskytovatelů a partnerů, kteří musí taky splňovat požadavky na certifikáty před konfigurací VPN pro aplikaci. Další informace najdete v článku [nastavení virtuální privátní sítě (VPN) pro zařízení s iOS/iPadOS v Intune na aplikaci](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Další informace o všech typech připojení VPN v Intune najdete v článku [Vytvoření profilů VPN pro připojení k SERVERŮM VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**připojení k síti VPN s iOS na vyžádání se při přístupu k nakonfigurované doméně nespouští**

Chcete-li otestovat nastavení automatického připojení VPN, nastavte následující hodnoty:

Chci udělat následující: **vyhodnoťte každý pokus o připojení** . 

Zvolte, jestli se chcete připojit: v **případě potřeby**

Když uživatelé přistupují k těmto doménám: název **cílové** *domény*

Pokud tato konfigurace není úspěšná, přidejte následující prvek:

Pokud je tato adresa URL nedostupná, vynuťte připojení sítě VPN: **BADURL**