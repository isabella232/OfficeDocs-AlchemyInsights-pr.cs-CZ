---
title: Používání e-mailových profilů s Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554843"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="3064a-102">Používání e-mailových profilů s Intune</span><span class="sxs-lookup"><span data-stu-id="3064a-102">Using email profiles with Intune</span></span>

<span data-ttu-id="3064a-103">Intune se dá použít k vytvoření a nasazení e-mailových profilů pro nativního (integrovaného) e-mailového klienta na platformách více zařízení.</span><span class="sxs-lookup"><span data-stu-id="3064a-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="3064a-104">Informace o některých omezeních spojených s e-mailovými profily, včetně způsobu zpracování stavu existujících profilů a odebrání e-mailových profilů, najdete v tématu [Přidání nastavení e-mailu do zařízení pomocí Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="3064a-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="3064a-105">Další informace o vytváření e-mailových profilů pro jednotlivé platformy zařízení najdete v tématu:</span><span class="sxs-lookup"><span data-stu-id="3064a-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="3064a-106">Nastavení zařízení Android pro konfiguraci e-mailu, ověřování a synchronizace v Intune</span><span class="sxs-lookup"><span data-stu-id="3064a-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="3064a-107">Přidání nastavení e-mailu pro zařízení s iOS a iPadOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3064a-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="3064a-108">Nastavení e-mailového profilu v Microsoft Intune pro zařízení s Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="3064a-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="3064a-109">Nastavení e-mailového profilu pro zařízení s Windows 10 v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3064a-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="3064a-110">**Běžný problém se synchronizací**</span><span class="sxs-lookup"><span data-stu-id="3064a-110">**Common syncing issue**</span></span>

<span data-ttu-id="3064a-111">**E-mailový profil KNOX v systému Android zabraňuje synchronizaci kontaktů, kalendářů a úkolů uživatelů s uživatelskými zařízeními.**</span><span class="sxs-lookup"><span data-stu-id="3064a-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="3064a-112">E-mailový profil KNOX v systému Android KNOX nabízí správci možnost rozhodnout, které typy obsahu jsou synchronizovány se zařízením, a to tak, že každý z nich bude povolen.</span><span class="sxs-lookup"><span data-stu-id="3064a-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="3064a-113">Pokud je nastavení pro některý z typů obsahu nastaveno na **Možnost Není nakonfigurováno** (výchozí), tento typ obsahu se automaticky nesynchronizuje.</span><span class="sxs-lookup"><span data-stu-id="3064a-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="3064a-114">Uživatel může povolit typ obsahu, který chce přímo na zařízení ručně, ale tato konfigurace je přepsána nastavením zásad Intune a synchronizace se zastaví pro tento typ obsahu.</span><span class="sxs-lookup"><span data-stu-id="3064a-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

