---
title: Řešení potíží s nasazením certifikátu ověřování klienta
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020797"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Řešení potíží s nasazením certifikátu ověřování klienta

Profily klientských certifikátů Intune NDES/SCEP a PKCS/PFX se běžně používají společně s jinými typy profilů, jako je Wifi, VPN a e-mail, aby se uživatelé mohly ověřovat na podnikové prostředky. Pokud jsou tyto typy profilů propojené s profilem klientského certifikátu, závisí na úspěšném nasazení tohoto profilu.

Počáteční nastavení infrastruktury a přidružená konfigurace profilu klientského certifikátu často vyžadují řešení potíží. Podrobný průvodce úspěšným nastavením konektoru NDES a pokyny k řešení potíží s nasazením certifikátů najdete v těchto článku: 

- [Konfigurace infrastruktury pro podporu SCEP pomocí Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Přehled řešení potíží s profily certifikátů SCEP pomocí Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

K ověření konfigurace použijte odkazované skripty powershellu. Další informace najdete v článku [Ověřovací skripty konektoru certifikátu Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Další běžné problémy**

**Když se pokusím nainstalovat konektor certifikátu Intune na server konektoru NDES, zobrazí se zpráva "Heslo v žádosti o certifikát nelze ověřit. Možná už byl použit. Získejte nové heslo pro odeslání s touto žádostí."**  

Tato zpráva znamená, že musíte spustit instalaci konektoru certifikátu jako správce.

V některých prostředích musí servery, na kterých běží certifikát Intune, používat proxy server pro připojení k Intune, a proto musí Konektor certifikátů používat proxy server. Za určitých okolností konektor NDES ignoruje nakonfigurovaná nastavení proxy serveru a může být nutné nakonfigurovat nastavení proxy serveru v kontextu zabezpečení LocalSystem. 
 
Řešením je spustit Internet Explorer jako SYSTÉM a nakonfigurovat proxy server v IE. Po restartování služby Konektor Intune se konektor NDES připojí k Intune.

**Uživatelská zařízení už od NDES nebírají certifikáty SCEP.**

Je možné, že vypršela platnost certifikátu ověření klienta vydaného serveru NDES a zadaný během instalace konektoru služby NDES nebo chybí. Řešení: 
 
1. Odinstalujte konektor NDES.  
2. Pomocí těchto podrobností můžete požádat o nové ověřování klienta nebo ověřovací certifikát serveru: 
 
    - Název předmětu: CN=externí plně kvalifikovaný název domény  
    - Alternativní název předmětu (oba jsou povinné): DNS=externí plně kvalifikovaný název domény, DNS=interní plně kvalifikovaný název domény 
 
3. Znovu nainstalujte konektor NDES s novým certifikátem.