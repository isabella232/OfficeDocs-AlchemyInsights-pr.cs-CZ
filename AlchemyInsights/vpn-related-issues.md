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
# <a name="vpn-related-issues"></a><span data-ttu-id="53061-102">Problémy související se sítí VPN</span><span class="sxs-lookup"><span data-stu-id="53061-102">VPN related issues</span></span>

<span data-ttu-id="53061-103">Úspěšná implementace připojení VPN pro klienty MDM závisí na nasazeném profilu, který správně odráží požadavky infrastruktury VPN.</span><span class="sxs-lookup"><span data-stu-id="53061-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="53061-104">Příslušné možnosti pro klientské platformy, které zkoumáte, najdete v tématu:</span><span class="sxs-lookup"><span data-stu-id="53061-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="53061-105">Nastavení zařízení s Windows 10 a celoplošným Holografickím přidání připojení VPN pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="53061-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="53061-106">Přidání nastavení sítě VPN pro zařízení s iOS a iPadOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="53061-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="53061-107">Nastavení zařízení s Androidem pro konfiguraci VPN v Intune</span><span class="sxs-lookup"><span data-stu-id="53061-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="53061-108">Přidání nastavení sítě VPN na zařízení macOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="53061-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="53061-109">Pokud váš profil sítě VPN používá ověřování založené na certifikátech, ujistěte se, že jsou profily certifikátů kořenového certifikátu a ověřování klientů propojené se svým profilem VPN úspěšně nasazené.</span><span class="sxs-lookup"><span data-stu-id="53061-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="53061-110">**Běžné problémy**</span><span class="sxs-lookup"><span data-stu-id="53061-110">**Common Issues**</span></span>

<span data-ttu-id="53061-111">**Na zařízení je nasazený profil sítě VPN. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k síti VPN.**</span><span class="sxs-lookup"><span data-stu-id="53061-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="53061-112">Úspěšný stav znamená, že v Intune se profil úspěšně nasadil jako nakonfigurovaný.</span><span class="sxs-lookup"><span data-stu-id="53061-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="53061-113">Tato konfigurace ale nemusí odpovídat vašim požadavkům na síť nebo ověřování.</span><span class="sxs-lookup"><span data-stu-id="53061-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="53061-114">Další podrobnosti o pokusu o připojení najdete v protokolech v tématu infrastruktura a ověřování (na serveru VPN a serveru NPS/RADIUS).</span><span class="sxs-lookup"><span data-stu-id="53061-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="53061-115">Pro shromáždění a kontrolu protokolů může být potřeba pracovat se svým týmem infrastruktury sítě nebo s dodavatelem VPN jiného výrobce.</span><span class="sxs-lookup"><span data-stu-id="53061-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="53061-116">**Když nakonfigurujem vlastní připojení VPN pro iOS, funkce VPN pro jednotlivé aplikace není dostupná.**</span><span class="sxs-lookup"><span data-stu-id="53061-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="53061-117">Připojení VPN pro zařízení s iOS v Intune je v současné době dostupné pro konkrétní seznam poskytovatelů a partnerů, kteří musí taky splňovat požadavky na certifikáty před konfigurací VPN pro aplikaci.</span><span class="sxs-lookup"><span data-stu-id="53061-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="53061-118">Další informace najdete v článku [nastavení virtuální privátní sítě (VPN) pro zařízení s iOS/iPadOS v Intune na aplikaci](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="53061-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="53061-119">Další informace o všech typech připojení VPN v Intune najdete v článku [Vytvoření profilů VPN pro připojení k SERVERŮM VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="53061-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="53061-120">**připojení k síti VPN s iOS na vyžádání se při přístupu k nakonfigurované doméně nespouští**</span><span class="sxs-lookup"><span data-stu-id="53061-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="53061-121">Chcete-li otestovat nastavení automatického připojení VPN, nastavte následující hodnoty:</span><span class="sxs-lookup"><span data-stu-id="53061-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="53061-122">Chci udělat následující: **vyhodnoťte každý pokus o připojení** .</span><span class="sxs-lookup"><span data-stu-id="53061-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="53061-123">Zvolte, jestli se chcete připojit: v **případě potřeby**</span><span class="sxs-lookup"><span data-stu-id="53061-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="53061-124">Když uživatelé přistupují k těmto doménám: název **cílové** *domény*</span><span class="sxs-lookup"><span data-stu-id="53061-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="53061-125">Pokud tato konfigurace není úspěšná, přidejte následující prvek:</span><span class="sxs-lookup"><span data-stu-id="53061-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="53061-126">Pokud je tato adresa URL nedostupná, vynuťte připojení sítě VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="53061-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>