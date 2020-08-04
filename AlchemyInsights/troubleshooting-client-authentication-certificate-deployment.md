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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="55b18-102">Poradce při potížích s nasazením certifikátu ověření klienta</span><span class="sxs-lookup"><span data-stu-id="55b18-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="55b18-103">Profily klientských certifikátů Intune NDES/SCEP a PKCS/PFX se běžně používají ve spojení s dalšími typy profilů, jako je Wifi, VPN a e-mail, aby uživatelé mohli ověřovat firemní prostředky.</span><span class="sxs-lookup"><span data-stu-id="55b18-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="55b18-104">Pokud jsou tyto typy profilů propojeny s profilem klientského certifikátu, závisí na úspěšném nasazení tohoto profilu.</span><span class="sxs-lookup"><span data-stu-id="55b18-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="55b18-105">Počáteční nastavení infrastruktury a přidružená konfigurace profilu klientského certifikátu často vyžadují řešení potíží.</span><span class="sxs-lookup"><span data-stu-id="55b18-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="55b18-106">Podrobný průvodce úspěšnou instalací konektoru NDES a pokyny pro řešení potíží s cílem izolovat problémy s nasazením certifikátu naleznete v následujících tématech:</span><span class="sxs-lookup"><span data-stu-id="55b18-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="55b18-107">Konfigurace infrastruktury pro podporu SCEP pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="55b18-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="55b18-108">Přehled řešení potíží s profily certifikátů SCEP pomocí Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="55b18-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="55b18-109">K ověření konfigurace použijte odkazované skripty prostředí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55b18-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="55b18-110">Další informace najdete v tématu [Ověřovací skripty konektoru intune certifikátu](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="55b18-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="55b18-111">**Další běžné problémy**</span><span class="sxs-lookup"><span data-stu-id="55b18-111">**Other common issues**</span></span>

<span data-ttu-id="55b18-112">**Při pokusu o instalaci konektoru certifikátu Intune na konektoru NDES server, zobrazí se zpráva, "heslo v žádosti o certifikát nelze ověřit. Možná už byl použit. Získat nové heslo k odeslání s touto žádostí."**</span><span class="sxs-lookup"><span data-stu-id="55b18-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="55b18-113">Tato zpráva znamená, že je třeba spustit instalaci konektoru certifikátu jako správce.</span><span class="sxs-lookup"><span data-stu-id="55b18-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="55b18-114">V některých prostředích musí servery, na kterých je spuštěn certifikát Intune, používat k intune proxy server, a proto musí konektor certifikátu používat proxy server.</span><span class="sxs-lookup"><span data-stu-id="55b18-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="55b18-115">V některých případech konektor NDES ignoruje nakonfigurované nastavení proxy serveru a může být nutné nakonfigurovat nastavení proxy serveru při spuštění v kontextu zabezpečení LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="55b18-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="55b18-116">Řešením je spustit aplikaci Internet Explorer jako SYSTEM a nakonfigurovat proxy server v aplikaci InternetE.</span><span class="sxs-lookup"><span data-stu-id="55b18-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="55b18-117">Po restartování služby konektoru Intune se konektor NDES připojí k Intune.</span><span class="sxs-lookup"><span data-stu-id="55b18-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="55b18-118">**Uživatelská zařízení již nedostávají certifikáty SCEP od sítě NDES.**</span><span class="sxs-lookup"><span data-stu-id="55b18-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="55b18-119">Je možné, že certifikát ověřování klienta vydaný serveru NDES a zadaný během instalace konektoru NDES vypršel nebo chybí.</span><span class="sxs-lookup"><span data-stu-id="55b18-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="55b18-120">Chcete-li vyřešit:</span><span class="sxs-lookup"><span data-stu-id="55b18-120">To resolve:</span></span> 
 
1. <span data-ttu-id="55b18-121">Odinstalujte konektor NDES.</span><span class="sxs-lookup"><span data-stu-id="55b18-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="55b18-122">Pomocí těchto údajů můžete požádat o nový certifikát ověřování klienta nebo ověření serveru:</span><span class="sxs-lookup"><span data-stu-id="55b18-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="55b18-123">Název subjektu: CN=externí fqdn</span><span class="sxs-lookup"><span data-stu-id="55b18-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="55b18-124">Alternativní název předmětu (oba jsou povinné): DNS=externí fqdn, DNS=interní fqdn</span><span class="sxs-lookup"><span data-stu-id="55b18-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="55b18-125">Přeinstalujte konektor NDES s novým certifikátem.</span><span class="sxs-lookup"><span data-stu-id="55b18-125">Reinstall the NDES connector with the new certificate.</span></span>