---
title: Poradce při potížích s nasazením certifikátu ověření klienta
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554855"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Poradce při potížích s nasazením certifikátu ověření klienta

Profily klientských certifikátů Intune NDES/SCEP a PKCS/PFX se běžně používají ve spojení s dalšími typy profilů, jako je Wifi, VPN a e-mail, aby uživatelé mohli ověřovat firemní prostředky. Pokud jsou tyto typy profilů propojeny s profilem klientského certifikátu, závisí na úspěšném nasazení tohoto profilu.

Počáteční nastavení infrastruktury a přidružená konfigurace profilu klientského certifikátu často vyžadují řešení potíží. Podrobný průvodce úspěšnou instalací konektoru NDES a pokyny pro řešení potíží s cílem izolovat problémy s nasazením certifikátu naleznete v následujících tématech: 

- [Konfigurace infrastruktury pro podporu SCEP pomocí Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Přehled řešení potíží s profily certifikátů SCEP pomocí Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

K ověření konfigurace použijte odkazované skripty prostředí PowerShell. Další informace najdete v tématu [Ověřovací skripty konektoru intune certifikátu](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Další běžné problémy**

**Při pokusu o instalaci konektoru certifikátu Intune na konektoru NDES server, zobrazí se zpráva, "heslo v žádosti o certifikát nelze ověřit. Možná už byl použit. Získat nové heslo k odeslání s touto žádostí."**  

Tato zpráva znamená, že je třeba spustit instalaci konektoru certifikátu jako správce.

V některých prostředích musí servery, na kterých je spuštěn certifikát Intune, používat k intune proxy server, a proto musí konektor certifikátu používat proxy server. V některých případech konektor NDES ignoruje nakonfigurované nastavení proxy serveru a může být nutné nakonfigurovat nastavení proxy serveru při spuštění v kontextu zabezpečení LocalSystem. 
 
Řešením je spustit aplikaci Internet Explorer jako SYSTEM a nakonfigurovat proxy server v aplikaci InternetE. Po restartování služby konektoru Intune se konektor NDES připojí k Intune.

**Uživatelská zařízení již nedostávají certifikáty SCEP od sítě NDES.**

Je možné, že certifikát ověřování klienta vydaný serveru NDES a zadaný během instalace konektoru NDES vypršel nebo chybí. Chcete-li vyřešit: 
 
1. Odinstalujte konektor NDES.  
2. Pomocí těchto údajů můžete požádat o nový certifikát ověřování klienta nebo ověření serveru: 
 
    - Název subjektu: CN=externí fqdn  
    - Alternativní název předmětu (oba jsou povinné): DNS=externí fqdn, DNS=interní fqdn 
 
3. Přeinstalujte konektor NDES s novým certifikátem.