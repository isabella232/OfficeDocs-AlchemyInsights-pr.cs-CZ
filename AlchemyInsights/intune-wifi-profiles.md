---
title: Intune profily Wi-Fi
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696254"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="f5664-102">Intune profily Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="f5664-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="f5664-103">Úspěšná implementace připojení Wi-Fi pro klienty MDM závisí na správně nasazeném profilu, který odráží požadavky podnikové infrastruktury Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f5664-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="f5664-104">Pokud chcete zkontrolovat příslušná nastavení pro klientské platformy, které zkoumáte, přečtěte si téma:</span><span class="sxs-lookup"><span data-stu-id="f5664-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="f5664-105">Přidání nastavení Wi-Fi pro zařízení s Androidem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f5664-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="f5664-106">Přidání nastavení Wi-Fi pro podniková vyhrazená a plně spravovaná zařízení s Androidem v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f5664-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="f5664-107">Přidání nastavení Wi-Fi pro zařízení s iOS a iPadOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f5664-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="f5664-108">Přidání nastavení Wi-Fi pro Windows 10 a novější zařízení v Intune</span><span class="sxs-lookup"><span data-stu-id="f5664-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="f5664-109">Import nastavení Wi-Fi pro zařízení s Windows v Intune</span><span class="sxs-lookup"><span data-stu-id="f5664-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="f5664-110">**Běžné problémy**</span><span class="sxs-lookup"><span data-stu-id="f5664-110">**Common Issues**</span></span>

<span data-ttu-id="f5664-111">**Zavádím profil sítě Wi-Fi, který je závislý na nasazeném certifikátu zadaném v profilu sítě Wi-Fi. Konfigurační profily však zobrazují chybový stav.**</span><span class="sxs-lookup"><span data-stu-id="f5664-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="f5664-112">Zkontrolujte, že vaše zařízení certifikát obdržel.</span><span class="sxs-lookup"><span data-stu-id="f5664-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="f5664-113">V Intune přejděte na **všechna zařízení** a vyberte zařízení > **konfiguraci zařízení**.</span><span class="sxs-lookup"><span data-stu-id="f5664-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="f5664-114">Zkontrolujte, jestli jsou všechny očekávané profily uvedené a v úspěšném stavu.</span><span class="sxs-lookup"><span data-stu-id="f5664-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="f5664-115">Pokud máte v řetězci certifikátu zprostředkující certifikáty, ujistěte se, že jsou na zařízení s Androidem nasazené.</span><span class="sxs-lookup"><span data-stu-id="f5664-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="f5664-116">Pokud chcete zkontrolovat stav certifikátu, přejděte na **konfigurační**  >  **profily**zařízení  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="f5664-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="f5664-117">Pokud se vám pořád zobrazují chyby, podívejte se na postupy a oddíly řešení potíží.</span><span class="sxs-lookup"><span data-stu-id="f5664-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="f5664-118">Další informace najdete v článku [o řešení potíží s profily certifikátů SCEP přes Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f5664-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="f5664-119">**Nasadil (a) profil sítě Wi-Fi na zařízení. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="f5664-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="f5664-120">Úspěšný stav znamená, že v Intune se profil úspěšně nasadil jako nakonfigurovaný.</span><span class="sxs-lookup"><span data-stu-id="f5664-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="f5664-121">Tato konfigurace ale nemusí odpovídat vašim požadavkům na síť nebo ověřování.</span><span class="sxs-lookup"><span data-stu-id="f5664-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="f5664-122">Další podrobnosti o pokusu o připojení najdete v protokolech v tématu infrastruktura a ověřování (na řadiči přístupových bodů sítě Wi-Fi a serveru NPS nebo RADIUS).</span><span class="sxs-lookup"><span data-stu-id="f5664-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="f5664-123">Možná budete muset pracovat s týmem infrastruktury sítě nebo s poskytovatelem Wi-Fi jiného výrobce, abyste mohli shromáždit a zkontrolovat protokoly.</span><span class="sxs-lookup"><span data-stu-id="f5664-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>