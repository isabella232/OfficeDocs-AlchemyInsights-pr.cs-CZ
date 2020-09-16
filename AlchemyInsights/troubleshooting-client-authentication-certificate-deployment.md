---
title: Řešení potíží s nasazením certifikátu ověření klienta
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658979"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Řešení potíží s nasazením certifikátu ověření klienta

V Intune – profily pro certifikáty klienta NDES/SCEP a PKCS/PFX se běžně používají ve spojení s jinými typy profilů, jako jsou WiFi, VPN a e-mail, aby uživatelé mohli ověřovat firemní prostředky. Pokud jsou tyto typy profilů propojené s profilem klientského certifikátu, závisejí na úspěšném nasazení tohoto profilu.

Počáteční nastavení infrastruktury a související konfigurace profilu klientského certifikátu často vyžadují řešení potíží. Podrobný průvodce pro úspěšné nastavení NDES Connectoru a pokyny pro odstraňování potíží s nasazením certifikátů najdete v těchto tématech: 

- [Konfigurace infrastruktury pro podporu SCEP s Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Základní informace o řešení potíží s profily certifikátů SCEP přes Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Pomocí odkazovaných skriptů PowerShellu můžete ověřit konfiguraci. Další informace najdete v článku [ověřovací skripty konektoru Certificate Connector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Další běžné problémy**

**Když se pokusím nainstalovat Certificate Tune na serveru NDES Connector, zobrazí se zpráva "heslo v žádosti o certifikát nelze ověřit. Pravděpodobně už byl použit. Získejte nové heslo pro odeslání s touto žádostí. "**  

Tato zpráva znamená, že musíte spustit instalaci Certificate Connectoru jako správce.

V některých prostředích se musí servery, na kterých běží certifikát Intune, použít proxy server, aby se připojil k Intune, a aby mohl Certificate Connector používat proxy server. V některých případech konektor NDES Connector ignoruje konfigurované nastavení proxy a může být potřeba ke konfiguraci nastavení proxy serveru při běhu v kontextu zabezpečení účtu LocalSystem. 
 
Řešením je spustit Internet Explorer jako systém a nakonfigurovat proxy server v aplikaci IE. Po restartování služby konektoru Intune se k Intune připojí konektor NDES Connector.

**Uživatelská zařízení už nepodporují certifikáty SCEP ze služby NDES.**

Je možné, že certifikát pro ověření klienta vydaný pro server NDES a zadaný během instalace NDES Connector vypršel nebo chybí. Řešení: 
 
1. Odinstalujte NDES Connector.  
2. K vyžádání nového ověřování klienta nebo ověřovacího certifikátu serveru použijte tyto podrobnosti: 
 
    - Název předmětu: CN = externí plně kvalifikovaný název domény  
    - Alternativní název subjektu (vyžaduje se): DNS = externí plně kvalifikovaný název domény, DNS = vnitřní plně kvalifikovaný název domény 
 
3. Znovu nainstalujte NDES Connector s novým certifikátem.