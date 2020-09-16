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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="f6b37-102">Řešení potíží s nasazením certifikátu ověření klienta</span><span class="sxs-lookup"><span data-stu-id="f6b37-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="f6b37-103">V Intune – profily pro certifikáty klienta NDES/SCEP a PKCS/PFX se běžně používají ve spojení s jinými typy profilů, jako jsou WiFi, VPN a e-mail, aby uživatelé mohli ověřovat firemní prostředky.</span><span class="sxs-lookup"><span data-stu-id="f6b37-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="f6b37-104">Pokud jsou tyto typy profilů propojené s profilem klientského certifikátu, závisejí na úspěšném nasazení tohoto profilu.</span><span class="sxs-lookup"><span data-stu-id="f6b37-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="f6b37-105">Počáteční nastavení infrastruktury a související konfigurace profilu klientského certifikátu často vyžadují řešení potíží.</span><span class="sxs-lookup"><span data-stu-id="f6b37-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="f6b37-106">Podrobný průvodce pro úspěšné nastavení NDES Connectoru a pokyny pro odstraňování potíží s nasazením certifikátů najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="f6b37-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="f6b37-107">Konfigurace infrastruktury pro podporu SCEP s Intune</span><span class="sxs-lookup"><span data-stu-id="f6b37-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="f6b37-108">Základní informace o řešení potíží s profily certifikátů SCEP přes Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f6b37-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="f6b37-109">Pomocí odkazovaných skriptů PowerShellu můžete ověřit konfiguraci.</span><span class="sxs-lookup"><span data-stu-id="f6b37-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="f6b37-110">Další informace najdete v článku [ověřovací skripty konektoru Certificate Connector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="f6b37-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="f6b37-111">**Další běžné problémy**</span><span class="sxs-lookup"><span data-stu-id="f6b37-111">**Other common issues**</span></span>

<span data-ttu-id="f6b37-112">**Když se pokusím nainstalovat Certificate Tune na serveru NDES Connector, zobrazí se zpráva "heslo v žádosti o certifikát nelze ověřit. Pravděpodobně už byl použit. Získejte nové heslo pro odeslání s touto žádostí. "**</span><span class="sxs-lookup"><span data-stu-id="f6b37-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="f6b37-113">Tato zpráva znamená, že musíte spustit instalaci Certificate Connectoru jako správce.</span><span class="sxs-lookup"><span data-stu-id="f6b37-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="f6b37-114">V některých prostředích se musí servery, na kterých běží certifikát Intune, použít proxy server, aby se připojil k Intune, a aby mohl Certificate Connector používat proxy server.</span><span class="sxs-lookup"><span data-stu-id="f6b37-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="f6b37-115">V některých případech konektor NDES Connector ignoruje konfigurované nastavení proxy a může být potřeba ke konfiguraci nastavení proxy serveru při běhu v kontextu zabezpečení účtu LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="f6b37-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="f6b37-116">Řešením je spustit Internet Explorer jako systém a nakonfigurovat proxy server v aplikaci IE.</span><span class="sxs-lookup"><span data-stu-id="f6b37-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="f6b37-117">Po restartování služby konektoru Intune se k Intune připojí konektor NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="f6b37-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="f6b37-118">**Uživatelská zařízení už nepodporují certifikáty SCEP ze služby NDES.**</span><span class="sxs-lookup"><span data-stu-id="f6b37-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="f6b37-119">Je možné, že certifikát pro ověření klienta vydaný pro server NDES a zadaný během instalace NDES Connector vypršel nebo chybí.</span><span class="sxs-lookup"><span data-stu-id="f6b37-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="f6b37-120">Řešení:</span><span class="sxs-lookup"><span data-stu-id="f6b37-120">To resolve:</span></span> 
 
1. <span data-ttu-id="f6b37-121">Odinstalujte NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="f6b37-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="f6b37-122">K vyžádání nového ověřování klienta nebo ověřovacího certifikátu serveru použijte tyto podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="f6b37-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="f6b37-123">Název předmětu: CN = externí plně kvalifikovaný název domény</span><span class="sxs-lookup"><span data-stu-id="f6b37-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="f6b37-124">Alternativní název subjektu (vyžaduje se): DNS = externí plně kvalifikovaný název domény, DNS = vnitřní plně kvalifikovaný název domény</span><span class="sxs-lookup"><span data-stu-id="f6b37-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="f6b37-125">Znovu nainstalujte NDES Connector s novým certifikátem.</span><span class="sxs-lookup"><span data-stu-id="f6b37-125">Reinstall the NDES connector with the new certificate.</span></span>