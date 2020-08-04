---
title: Problémy související s VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554839"
---
# <a name="vpn-related-issues"></a>Problémy související s VPN

Úspěšná implementace připojení VPN pro klienty MDM závisí na nasazeném profilu, který správně odráží požadavky infrastruktury VPN. Příslušná nastavení pro klientské platformy, které zkoumáte, naleznete v následujících tématech: 

[Nastavení systému Windows 10 a holografického zařízení windows pro přidání připojení VPN pomocí Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Přidání nastavení VPN na zařízeních s iOS a iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Nastavení zařízení Android pro konfiguraci sítě VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Přidání nastavení VPN na zařízeních s macOS v Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Pokud váš profil VPN používá ověřování založené na certifikátech, ujistěte se, že kořenový certifikát a profily certifikátů ověřování klienta propojené s profilem VPN jsou úspěšně nasazeny.

**Běžné problémy**

**Do zařízení jsem nasadil profil VPN. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k VPN.**

Úspěšný stav znamená, že Intune úspěšně nasadil profil tak, jak byl nakonfigurovaný. Tyto konfigurace však nemusí odpovídat požadavkům na síť nebo ověřování. Další podrobnosti o pokusu o připojení naleznete v protokolech v infrastruktuře a ověřovací službě (na serveru VPN a serveru NPS/Radius). Možná budete muset spolupracovat s týmem síťové infrastruktury nebo s dodavatelem VPN jiného výrobce, abyste shromáždili a zkontrolovali protokoly.

**Když nakonfiguruji vlastní VPN pro iOS, funkce VPN pro aplikaci není k dispozici.**

VPN pro iOS pro aplikace v Intune je momentálně dostupná konkrétnímu seznamu zprostředkovatelů a partnerů, kteří musí před konfigurací VPN pro jednotlivé aplikace také splňovat požadavky certifikátu. Další informace najdete v [tématu Nastavení virtuální privátní sítě (VPN) pro virtuální privátní síť pro aplikaci v aplikaci iOS/iPadOS v Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Další informace o všech typech připojení VPN v Intune najdete v [tématu Vytvoření profilů VPN pro připojení k serverům VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**Síť VPN na vyžádání v systému iOS se neaktivuje, když je přístup k nakonfigurované doméně**

Chcete-li otestovat automatické nastavení sítě VPN, nastavte následující hodnoty:

Chci provést následující kroky: **Vyhodnotit každý pokus o připojení** 

Volba, zda se má připojit: **Připojit se v případě potřeby**

Když uživatelé přistupuje k těmto doménám: **název cílové** *domény*

Pokud výše uvedená konfigurace není úspěšná, přidejte následující prvek:

Pokud je tato adresa URL nedostupná, vynutit připojení VPN: **BADURL**