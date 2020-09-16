---
title: Používání profilů e-mailů s Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653281"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="3a93d-102">Používání profilů e-mailů s Intune</span><span class="sxs-lookup"><span data-stu-id="3a93d-102">Using email profiles with Intune</span></span>

<span data-ttu-id="3a93d-103">Intune se dá použít k vytvoření a nasazení profilů e-mailů pro nativní (vestavěný) e-mailový klient na více platformách zařízení.</span><span class="sxs-lookup"><span data-stu-id="3a93d-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="3a93d-104">Informace o některých omezeních souvisejících s e-mailovými profily, včetně způsobu, jakým se řídí přítomnost stávajících profilů a jak odebrat profily e-mailu, najdete v článku [Přidání nastavení e-mailu do zařízení pomocí Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="3a93d-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="3a93d-105">Další informace o vytváření profilů e-mailů pro jednotlivé platformy zařízení najdete v těchto tématech:</span><span class="sxs-lookup"><span data-stu-id="3a93d-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="3a93d-106">Nastavení zařízení s Androidem pro konfiguraci e-mailů, ověřování a synchronizace v Intune</span><span class="sxs-lookup"><span data-stu-id="3a93d-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="3a93d-107">Přidání nastavení e-mailu pro zařízení s iOS a iPadOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3a93d-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="3a93d-108">Nastavení e-mailového profilu v Microsoft Intune pro zařízení s Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="3a93d-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="3a93d-109">Nastavení e-mailového profilu pro zařízení s Windows 10 v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3a93d-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="3a93d-110">**Běžný problém se synchronizací**</span><span class="sxs-lookup"><span data-stu-id="3a93d-110">**Common syncing issue**</span></span>

<span data-ttu-id="3a93d-111">**V e-mailovém profilu pro Android brání uživatelům, kalendářům a úkolům v synchronizaci s uživatelskými zařízeními.**</span><span class="sxs-lookup"><span data-stu-id="3a93d-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="3a93d-112">V e-mailovém profilu pro Android KNOX nabízí správce možnost rozhodnout se, které typy obsahu se budou synchronizovat, nastavením příslušných možností.</span><span class="sxs-lookup"><span data-stu-id="3a93d-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="3a93d-113">Pokud je nastavení libovolného typu obsahu nastaveno na **Nenakonfigurováno** (výchozí nastavení), nebude tento typ obsahu automaticky synchronizován.</span><span class="sxs-lookup"><span data-stu-id="3a93d-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="3a93d-114">Uživatel může povolit, aby typ obsahu, který mají být přímo v zařízení, byl v nastavení zásad Intune přepsán a synchronizace se u tohoto typu obsahu zastaví.</span><span class="sxs-lookup"><span data-stu-id="3a93d-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

