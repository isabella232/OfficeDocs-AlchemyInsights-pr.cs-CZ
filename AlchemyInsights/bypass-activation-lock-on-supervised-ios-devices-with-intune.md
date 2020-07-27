---
title: Obejít zámek aktivace na kontrolovaných zařízeních iOS s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423490"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="b7eef-102">Obejít zámek aktivace na kontrolovaných zařízeních iOS s Intune</span><span class="sxs-lookup"><span data-stu-id="b7eef-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="b7eef-103">Možnost obejít zámek aktivace na zařízeních se systémem iOS usnadňuje obnovení ze scénáře, kdy uživatel povolí zámek aktivace na podnikovém zařízení a pak opustí společnost.</span><span class="sxs-lookup"><span data-stu-id="b7eef-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="b7eef-104">Předpoklady k vynechání zámku aktivace zahrnují:</span><span class="sxs-lookup"><span data-stu-id="b7eef-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="b7eef-105">Zařízení je, že je "pod dohledem."</span><span class="sxs-lookup"><span data-stu-id="b7eef-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="b7eef-106">Zámek aktivace je úspěšně povolený pomocí zásad omezení zařízení iOS v Intune.</span><span class="sxs-lookup"><span data-stu-id="b7eef-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="b7eef-107">Kromě toho při vynechání zámku aktivace byste měli:</span><span class="sxs-lookup"><span data-stu-id="b7eef-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="b7eef-108">Fyzicky ovládni zařízení, které bylo vymazáno.</span><span class="sxs-lookup"><span data-stu-id="b7eef-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="b7eef-109">Před vydáním vymazání zkopírujte kód.</span><span class="sxs-lookup"><span data-stu-id="b7eef-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="b7eef-110">**Poznámka:** Kód vymazání nerozlišuje malá a velká písmena, takže znaky "-" nejsou vyžadovány.</span><span class="sxs-lookup"><span data-stu-id="b7eef-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="b7eef-111">Podrobnosti najdete v [tématu Vynechání zámku aktivace na zařízeních s iOS s Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="b7eef-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="b7eef-112">**Nejčastější dotazy**</span><span class="sxs-lookup"><span data-stu-id="b7eef-112">**FAQ**</span></span>

<span data-ttu-id="b7eef-113">Otázka: **Vydal jsem vzdálenou akci k odebrání firemních dat ze zařízení a nyní se zasekne ve stavu čekající na vyřízení.**</span><span class="sxs-lookup"><span data-stu-id="b7eef-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="b7eef-114">A: Pro vzdálené akce úspěšně dokončit cílové zařízení musí být online a v pořádku.</span><span class="sxs-lookup"><span data-stu-id="b7eef-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="b7eef-115">V následujících situacích zůstane vzdálená akce ve stavu čekající na vyřízení po dobu 30 dnů nebo dokud zařízení nepotvrdí příkaz, když zařízení:</span><span class="sxs-lookup"><span data-stu-id="b7eef-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="b7eef-116">Nemá připojení.</span><span class="sxs-lookup"><span data-stu-id="b7eef-116">Does not have connectivity.</span></span>
- <span data-ttu-id="b7eef-117">Ztratí svůj stav správy s Intune.</span><span class="sxs-lookup"><span data-stu-id="b7eef-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="b7eef-118">Pokud se domníváte, že zařízení se už nehlásí a že neodebere firemní data, vyberte Odstranit.</span><span class="sxs-lookup"><span data-stu-id="b7eef-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="b7eef-119">Odstraněním odeberete záznam zařízení, aby se už nezobával v seznamu zařízení Intune.</span><span class="sxs-lookup"><span data-stu-id="b7eef-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="b7eef-120">Aby se zařízení znovu aktivovalo, musí jeho uživatel zařízení znovu zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="b7eef-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="b7eef-121">Otázka: **Proč nejsou k dispozici určité vzdálené akce, které nelze použít?**</span><span class="sxs-lookup"><span data-stu-id="b7eef-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="b7eef-122">A: Ne všechny platformy podporují všechny akce vzdáleného zařízení.</span><span class="sxs-lookup"><span data-stu-id="b7eef-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="b7eef-123">Následující vzdálené akce jsou specifické pro platformu.</span><span class="sxs-lookup"><span data-stu-id="b7eef-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="b7eef-124">Vynechání zámku aktivace (pouze iOS)</span><span class="sxs-lookup"><span data-stu-id="b7eef-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="b7eef-125">Nový začátek (pouze windows)</span><span class="sxs-lookup"><span data-stu-id="b7eef-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="b7eef-126">Režim ztráty (pouze iOS)</span><span class="sxs-lookup"><span data-stu-id="b7eef-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="b7eef-127">Vyhledání zařízení (pouze iOS)</span><span class="sxs-lookup"><span data-stu-id="b7eef-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="b7eef-128">Restartování (pouze windows)</span><span class="sxs-lookup"><span data-stu-id="b7eef-128">Restart (Windows only)</span></span>

<span data-ttu-id="b7eef-129">Další podrobnosti o jednotlivých akcích najdete v [tématu Dostupné akce zařízení](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="b7eef-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>