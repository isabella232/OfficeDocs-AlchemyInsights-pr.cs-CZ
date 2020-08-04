---
title: Profily Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554856"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="c3420-102">Profily Wi-Fi Intune</span><span class="sxs-lookup"><span data-stu-id="c3420-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="c3420-103">Úspěšná implementace wi-fi připojení pro klienty MDM závisí na správně nasazeném profilu, který odráží požadavky podnikové infrastruktury Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c3420-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="c3420-104">Chcete-li zkontrolovat příslušná nastavení pro klientské platformy, které zkoumáte, naleznete v následujících tématech:</span><span class="sxs-lookup"><span data-stu-id="c3420-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="c3420-105">Přidání nastavení Wi-Fi pro zařízení se systémem Android v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c3420-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="c3420-106">Přidání nastavení Wi-Fi pro vyhrazená a plně spravovaná zařízení Android Enterprise v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c3420-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="c3420-107">Přidání nastavení Wi-Fi pro iOS a iPadOS zařízení v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c3420-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="c3420-108">Přidání nastavení Wi-Fi pro zařízení s Windows 10 a novějšími v Intune</span><span class="sxs-lookup"><span data-stu-id="c3420-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="c3420-109">Import nastavení Wi-Fi pro zařízení s Windows v Intune</span><span class="sxs-lookup"><span data-stu-id="c3420-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="c3420-110">**Běžné problémy**</span><span class="sxs-lookup"><span data-stu-id="c3420-110">**Common Issues**</span></span>

<span data-ttu-id="c3420-111">**Nasazuji profil Wi-Fi, který je závislý na nasazeném certifikátu určeném v profilu Wi-Fi. Konfigurační profily však zobrazují stav chyby.**</span><span class="sxs-lookup"><span data-stu-id="c3420-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="c3420-112">Zkontrolujte, zda zařízení obdrželo certifikát.</span><span class="sxs-lookup"><span data-stu-id="c3420-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="c3420-113">V Intune přejděte na **Všechna zařízení** a vyberte zařízení > **konfiguraci zařízení**.</span><span class="sxs-lookup"><span data-stu-id="c3420-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="c3420-114">Zkontrolujte, zda jsou uvedeny všechny očekávané profily a v úspěšném stavu.</span><span class="sxs-lookup"><span data-stu-id="c3420-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="c3420-115">Pokud máte v řetězu certifikátů zprostředkující certifikáty, ujistěte se, že jsou nasazené do zařízení s Androidem.</span><span class="sxs-lookup"><span data-stu-id="c3420-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="c3420-116">Chcete-li zkontrolovat stav certifikátu, **přejděte**na profily konfigurace zařízení  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="c3420-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="c3420-117">Pokud se chyby budou zobrazovat i nadále, přečtěte si části postupy a řešení potíží.</span><span class="sxs-lookup"><span data-stu-id="c3420-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="c3420-118">Další informace najdete v [tématu Přehled řešení potíží s profily certifikátů SCEP pomocí Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c3420-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="c3420-119">**Do zařízení jsem nasadil profil Wi-Fi. Intune ukazuje, že byl úspěšný, ale zařízení se nepřipojuje k Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="c3420-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="c3420-120">Úspěšný stav znamená, že Intune úspěšně nasadil profil tak, jak byl nakonfigurovaný.</span><span class="sxs-lookup"><span data-stu-id="c3420-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="c3420-121">Tyto konfigurace však nemusí odpovídat požadavkům na síť nebo ověřování.</span><span class="sxs-lookup"><span data-stu-id="c3420-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="c3420-122">Další podrobnosti o pokusu o připojení naleznete v protokolech v infrastruktuře a službě ověřování (na řadiči přístupových bodů Wi-Fi a serveru NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="c3420-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="c3420-123">Možná budete muset spolupracovat s týmem síťové infrastruktury nebo s externím dodavatelem Wi-Fi, abyste shromáždili a zkontrolovali protokoly.</span><span class="sxs-lookup"><span data-stu-id="c3420-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>