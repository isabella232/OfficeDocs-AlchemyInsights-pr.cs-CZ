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
# <a name="vpn-related-issues"></a><span data-ttu-id="f099a-102">Problémy související s VPN</span><span class="sxs-lookup"><span data-stu-id="f099a-102">VPN related issues</span></span>

<span data-ttu-id="f099a-103">Úspěšná implementace připojení VPN pro klienty MDM závisí na nasazeném profilu, který správně odráží požadavky infrastruktury VPN.</span><span class="sxs-lookup"><span data-stu-id="f099a-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="f099a-104">Příslušná nastavení pro klientské platformy, které zkoumáte, naleznete v následujících tématech:</span><span class="sxs-lookup"><span data-stu-id="f099a-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="f099a-105">Nastavení systému Windows 10 a holografického zařízení windows pro přidání připojení VPN pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="f099a-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="f099a-106">Přidání nastavení VPN na zařízeních s iOS a iPadOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f099a-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="f099a-107">Nastavení zařízení Android pro konfiguraci sítě VPN v Intune</span><span class="sxs-lookup"><span data-stu-id="f099a-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="f099a-108">Přidání nastavení VPN na zařízeních s macOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f099a-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="f099a-109">Pokud váš profil VPN používá ověřování založené na certifikátech, ujistěte se, že kořenový certifikát a profily certifikátů ověřování klienta propojené s profilem VPN jsou úspěšně nasazeny.</span><span class="sxs-lookup"><span data-stu-id="f099a-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="f099a-110">**Běžné problémy**</span><span class="sxs-lookup"><span data-stu-id="f099a-110">**Common Issues**</span></span>

<span data-ttu-id="f099a-111">**Do zařízení jsem nasadil profil VPN. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k VPN.**</span><span class="sxs-lookup"><span data-stu-id="f099a-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="f099a-112">Úspěšný stav znamená, že Intune úspěšně nasadil profil tak, jak byl nakonfigurovaný.</span><span class="sxs-lookup"><span data-stu-id="f099a-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="f099a-113">Tyto konfigurace však nemusí odpovídat požadavkům na síť nebo ověřování.</span><span class="sxs-lookup"><span data-stu-id="f099a-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="f099a-114">Další podrobnosti o pokusu o připojení naleznete v protokolech v infrastruktuře a ověřovací službě (na serveru VPN a serveru NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="f099a-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="f099a-115">Možná budete muset spolupracovat s týmem síťové infrastruktury nebo s dodavatelem VPN jiného výrobce, abyste shromáždili a zkontrolovali protokoly.</span><span class="sxs-lookup"><span data-stu-id="f099a-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="f099a-116">**Když nakonfiguruji vlastní VPN pro iOS, funkce VPN pro aplikaci není k dispozici.**</span><span class="sxs-lookup"><span data-stu-id="f099a-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="f099a-117">VPN pro iOS pro aplikace v Intune je momentálně dostupná konkrétnímu seznamu zprostředkovatelů a partnerů, kteří musí před konfigurací VPN pro jednotlivé aplikace také splňovat požadavky certifikátu.</span><span class="sxs-lookup"><span data-stu-id="f099a-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="f099a-118">Další informace najdete v [tématu Nastavení virtuální privátní sítě (VPN) pro virtuální privátní síť pro aplikaci v aplikaci iOS/iPadOS v Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="f099a-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="f099a-119">Další informace o všech typech připojení VPN v Intune najdete v [tématu Vytvoření profilů VPN pro připojení k serverům VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="f099a-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="f099a-120">**Síť VPN na vyžádání v systému iOS se neaktivuje, když je přístup k nakonfigurované doméně**</span><span class="sxs-lookup"><span data-stu-id="f099a-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="f099a-121">Chcete-li otestovat automatické nastavení sítě VPN, nastavte následující hodnoty:</span><span class="sxs-lookup"><span data-stu-id="f099a-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="f099a-122">Chci provést následující kroky: **Vyhodnotit každý pokus o připojení**</span><span class="sxs-lookup"><span data-stu-id="f099a-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="f099a-123">Volba, zda se má připojit: **Připojit se v případě potřeby**</span><span class="sxs-lookup"><span data-stu-id="f099a-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="f099a-124">Když uživatelé přistupuje k těmto doménám: **název cílové** *domény*</span><span class="sxs-lookup"><span data-stu-id="f099a-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="f099a-125">Pokud výše uvedená konfigurace není úspěšná, přidejte následující prvek:</span><span class="sxs-lookup"><span data-stu-id="f099a-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="f099a-126">Pokud je tato adresa URL nedostupná, vynutit připojení VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="f099a-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>