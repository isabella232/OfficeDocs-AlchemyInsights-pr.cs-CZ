---
title: Odebrání služby pozadí pro Microsoft Search v Bingu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816091"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="de6b8-102">Odebrání služby pozadí pro Microsoft Search v Bingu</span><span class="sxs-lookup"><span data-stu-id="de6b8-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="de6b8-103">Pokud chcete odebrat službu pozadí pro Microsoft Search v Bingu, můžete vyzkoušet následující prostředky nápravy:</span><span class="sxs-lookup"><span data-stu-id="de6b8-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="de6b8-104">Pokud se chcete vrátit k původnímu nastavení vyhledávacího webu, proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="de6b8-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="de6b8-105">a.</span><span class="sxs-lookup"><span data-stu-id="de6b8-105">a.</span></span> <span data-ttu-id="de6b8-106">Přepněte **přepínač Používat Bing jako výchozí vyhledávací [modul.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**</span><span class="sxs-lookup"><span data-stu-id="de6b8-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="de6b8-107">b.</span><span class="sxs-lookup"><span data-stu-id="de6b8-107">b.</span></span> <span data-ttu-id="de6b8-108">[Přejděte do Centra pro správu Microsoftu 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) a zrušte nastavení, které se týká všech uživatelů ve vaší organizaci.</span><span class="sxs-lookup"><span data-stu-id="de6b8-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="de6b8-109">Pokud chcete odebrat službu pozadí z jednotlivých zařízení, proveďte následující úkoly:</span><span class="sxs-lookup"><span data-stu-id="de6b8-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="de6b8-110">a.</span><span class="sxs-lookup"><span data-stu-id="de6b8-110">a.</span></span> <span data-ttu-id="de6b8-111">Zvolte **Ovládací panely > Programy > Programy a funkce**.</span><span class="sxs-lookup"><span data-stu-id="de6b8-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="de6b8-112">b.</span><span class="sxs-lookup"><span data-stu-id="de6b8-112">b.</span></span> <span data-ttu-id="de6b8-113">V seznamu nainstalovaných programů klikněte pravým tlačítkem myši na **Microsoft Search v Bingu** a potom klikněte na **Odinstalovat.**</span><span class="sxs-lookup"><span data-stu-id="de6b8-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="de6b8-114">Pokud chcete odebrat službu pozadí z více zařízení ve vaší organizaci, přihlaste se jako správce a ve skriptu spusťte následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="de6b8-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
