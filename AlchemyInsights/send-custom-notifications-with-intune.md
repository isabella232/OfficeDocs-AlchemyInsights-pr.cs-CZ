---
title: Odesílání vlastních oznámení pomocí Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720639"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="dbfee-102">Jak posílat vlastní upozornění uživatelům spravovaných zařízení s iOS a Androidem</span><span class="sxs-lookup"><span data-stu-id="dbfee-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="dbfee-103">Vlastní oznámení o Intune zpracovává aplikace Portál společnosti na zařízení uživatele.</span><span class="sxs-lookup"><span data-stu-id="dbfee-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="dbfee-104">Aplikace potom vytvoří nabízené oznámení na tomto zařízení.</span><span class="sxs-lookup"><span data-stu-id="dbfee-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="dbfee-105">Níže jsou požadavky na zařízení, které podporují přijímání vlastních oznámení, a pro aplikaci pak vytvoří nabízené oznámení:</span><span class="sxs-lookup"><span data-stu-id="dbfee-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="dbfee-106">Na zařízení musí být nainstalovaná aplikace Portál společnosti.</span><span class="sxs-lookup"><span data-stu-id="dbfee-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="dbfee-107">Zařízení musí povolit aplikaci Portál společnosti odesílat nabízená oznámení.</span><span class="sxs-lookup"><span data-stu-id="dbfee-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="dbfee-108">Když se aplikace nainstaluje nebo aktualizuje, vyzve uživatele k povolení oznámení.</span><span class="sxs-lookup"><span data-stu-id="dbfee-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="dbfee-109">Zařízení s Androidem musí být nainstalovaná služba Google Play.</span><span class="sxs-lookup"><span data-stu-id="dbfee-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="dbfee-110">Zařízení musí být zaregistrované s Intune.</span><span class="sxs-lookup"><span data-stu-id="dbfee-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="dbfee-111">Další informace včetně odesílání zpráv najdete v [dokumentaci k funkcím](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="dbfee-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
