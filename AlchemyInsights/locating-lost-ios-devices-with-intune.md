---
title: Vyhledání ztracených zařízení iOS pomocí Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439145"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="73382-102">Vyhledání ztracených zařízení iOS pomocí Intune</span><span class="sxs-lookup"><span data-stu-id="73382-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="73382-103">Povolení režimu ztráty na zařízení se systémem iOS umožňuje správci zobrazit na zamykací obrazovce zprávu a telefonní číslo kontaktu.</span><span class="sxs-lookup"><span data-stu-id="73382-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="73382-104">Po povolení režimu ztráty může správce použít akci Vyhledat zařízení k identifikaci fyzického umístění zařízení.</span><span class="sxs-lookup"><span data-stu-id="73382-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="73382-105">Akce Najít zařízení v Intune funguje se zařízeními s iOS a zobrazuje umístění konkrétního zařízení na mapě.</span><span class="sxs-lookup"><span data-stu-id="73382-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="73382-106">Použití této akce vyžaduje, aby se iOS zařízení nachyoduje v:</span><span class="sxs-lookup"><span data-stu-id="73382-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="73382-107">Režim pod dohledem</span><span class="sxs-lookup"><span data-stu-id="73382-107">Supervised mode</span></span>
- <span data-ttu-id="73382-108">Režim ztráty</span><span class="sxs-lookup"><span data-stu-id="73382-108">Lost mode</span></span>

<span data-ttu-id="73382-109">Další informace najdete v [tématu Povolení režimu ztráty na zařízeních iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-lost-mode) a [Vyhledání ztracených nebo odcizených zařízení iOS/iPadOS s Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="73382-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="73382-110">**Nejčastější dotazy**</span><span class="sxs-lookup"><span data-stu-id="73382-110">**FAQ**</span></span>

<span data-ttu-id="73382-111">Otázka: Vydal jsem vzdálenou akci k odebrání firemních dat ze zařízení a nyní se zasekne ve stavu čekající na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="73382-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="73382-112">A: Pro vzdálené akce úspěšně dokončit cílové zařízení musí být online a v pořádku.</span><span class="sxs-lookup"><span data-stu-id="73382-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="73382-113">V následujících situacích zůstane vzdálená akce ve stavu čekající na vyřízení po dobu 30 dnů nebo dokud zařízení příkaz nepotvrdí:</span><span class="sxs-lookup"><span data-stu-id="73382-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="73382-114">Pokud zařízení nemá připojení</span><span class="sxs-lookup"><span data-stu-id="73382-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="73382-115">Když zařízení ztratí svůj stav správy s Intune</span><span class="sxs-lookup"><span data-stu-id="73382-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="73382-116">Pokud se domníváte, že zařízení se už nehlásí a že nebude moct odebrat firemní data, vyberte Odstranit.</span><span class="sxs-lookup"><span data-stu-id="73382-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="73382-117">Odstraněním odeberete záznam zařízení, aby se už nezobával v seznamu zařízení Intune.</span><span class="sxs-lookup"><span data-stu-id="73382-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="73382-118">Pokud se zařízení znovu aktivuje, jeho uživatel jej bude muset znovu zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="73382-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="73382-119">Otázka: Proč nejsou k dispozici určité vzdálené akce, které nelze použít?</span><span class="sxs-lookup"><span data-stu-id="73382-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="73382-120">A: Ne všechny platformy podporují všechny akce vzdáleného zařízení.</span><span class="sxs-lookup"><span data-stu-id="73382-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="73382-121">Následující vzdálené akce jsou specifické pro platformu, takže jsou k dispozici pouze pro uvedené platformy.</span><span class="sxs-lookup"><span data-stu-id="73382-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="73382-122">Vynechání zámku aktivace (pouze iOS)</span><span class="sxs-lookup"><span data-stu-id="73382-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="73382-123">Nový začátek (pouze windows)</span><span class="sxs-lookup"><span data-stu-id="73382-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="73382-124">Režim ztráty (pouze iOS)</span><span class="sxs-lookup"><span data-stu-id="73382-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="73382-125">Vyhledání zařízení (pouze iOS)</span><span class="sxs-lookup"><span data-stu-id="73382-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="73382-126">Restartování (pouze windows)</span><span class="sxs-lookup"><span data-stu-id="73382-126">Restart (Windows only)</span></span>

<span data-ttu-id="73382-127">Další podrobnosti o jednotlivých akcích najdete v [tématu Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="73382-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>