---
title: Vyhledání ztracených zařízení s iOS s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675149"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="605c6-102">Vyhledání ztracených zařízení s iOS s Intune</span><span class="sxs-lookup"><span data-stu-id="605c6-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="605c6-103">Povolení režimu ztráty na zařízení s iOS umožňuje správci na zamykací obrazovce zobrazit zprávu a telefonní číslo.</span><span class="sxs-lookup"><span data-stu-id="605c6-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="605c6-104">Když je režim ztráty povolený, může správce pomocí akce najít zařízení identifikovat fyzické umístění zařízení.</span><span class="sxs-lookup"><span data-stu-id="605c6-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="605c6-105">Akce najít zařízení v Intune funguje se zařízeními s iOS, která ukazuje umístění určitého zařízení na mapě.</span><span class="sxs-lookup"><span data-stu-id="605c6-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="605c6-106">Použití této akce vyžaduje, aby bylo zařízení s iOS v:</span><span class="sxs-lookup"><span data-stu-id="605c6-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="605c6-107">Sledovaný režim</span><span class="sxs-lookup"><span data-stu-id="605c6-107">Supervised mode</span></span>
- <span data-ttu-id="605c6-108">Režim ztráty</span><span class="sxs-lookup"><span data-stu-id="605c6-108">Lost mode</span></span>

<span data-ttu-id="605c6-109">Další informace najdete v článku [Povolení režimu ztraceného zobrazení na zařízeních s iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-lost-mode) a [vyhledání ztracených nebo odcizených zařízení s iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="605c6-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="605c6-110">**Nejčastější dotazy**</span><span class="sxs-lookup"><span data-stu-id="605c6-110">**FAQ**</span></span>

<span data-ttu-id="605c6-111">Otázka: byla vydána vzdálená akce, která odebere firemní data ze zařízení a teď je ve stavu čekání na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="605c6-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="605c6-112">A: aby byla úspěšná vzdálená akce, musí být cílové zařízení online a v pořádku.</span><span class="sxs-lookup"><span data-stu-id="605c6-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="605c6-113">V následujících situacích zůstane vzdálená akce v nevyřízeném stavu po dobu 30 dnů nebo dokud zařízení nepotvrdí příkaz:</span><span class="sxs-lookup"><span data-stu-id="605c6-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="605c6-114">Pokud zařízení nemá připojení</span><span class="sxs-lookup"><span data-stu-id="605c6-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="605c6-115">Když zařízení ztratí stav správy s Intune</span><span class="sxs-lookup"><span data-stu-id="605c6-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="605c6-116">Pokud si myslíte, že zařízení už není v nerezervování, a že nepůjde odebrat data společnosti, vyberte Odstranit.</span><span class="sxs-lookup"><span data-stu-id="605c6-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="605c6-117">Odstraněním odeberete záznam zařízení, aby se už nezobrazoval v seznamu zařízení v Intune.</span><span class="sxs-lookup"><span data-stu-id="605c6-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="605c6-118">Pokud se zařízení opět stane aktivní, bude ho muset uživatel znovu zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="605c6-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="605c6-119">Otázka: Proč nejsou některé vzdálené akce pro mě k dispozici?</span><span class="sxs-lookup"><span data-stu-id="605c6-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="605c6-120">A: ne všechny platformy podporují všechny akce vzdálených zařízení.</span><span class="sxs-lookup"><span data-stu-id="605c6-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="605c6-121">Následující vzdálené akce jsou závislé na platformě, takže jsou k dispozici pouze pro uvedené platformy.</span><span class="sxs-lookup"><span data-stu-id="605c6-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="605c6-122">Vynechat zámek aktivace (jenom iOS)</span><span class="sxs-lookup"><span data-stu-id="605c6-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="605c6-123">Nové spuštění (jenom Windows)</span><span class="sxs-lookup"><span data-stu-id="605c6-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="605c6-124">Ztracené zobrazení (jenom iOS)</span><span class="sxs-lookup"><span data-stu-id="605c6-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="605c6-125">Vyhledání zařízení (jenom iOS)</span><span class="sxs-lookup"><span data-stu-id="605c6-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="605c6-126">Restartovat (jenom Windows)</span><span class="sxs-lookup"><span data-stu-id="605c6-126">Restart (Windows only)</span></span>

<span data-ttu-id="605c6-127">Další podrobnosti o jednotlivých akcích najdete v tématu [Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="605c6-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>