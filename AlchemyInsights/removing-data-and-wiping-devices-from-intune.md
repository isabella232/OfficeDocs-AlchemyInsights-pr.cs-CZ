---
title: Odebrání dat a vymazání zařízení z Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439154"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="e3d17-102">Odebrání dat a vymazání zařízení z Intune</span><span class="sxs-lookup"><span data-stu-id="e3d17-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="e3d17-103">Vzdálené akce Vyřazení zařízení a Vymazání zařízení lze použít k odebrání firemních dat spravovaných službou Intune nebo k obnovení továrního nastavení a vrácení zařízení do výchozího nastavení.</span><span class="sxs-lookup"><span data-stu-id="e3d17-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="e3d17-104">Přihlaste se ke správě zařízení Microsoft 365 a přejděte na **Zařízení**  >  **všechna zařízení**.</span><span class="sxs-lookup"><span data-stu-id="e3d17-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="e3d17-105">Vyberte zařízení, které chcete vymazat.</span><span class="sxs-lookup"><span data-stu-id="e3d17-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="e3d17-106">Vyberte typ vzdáleného vymazání, které chcete provést.</span><span class="sxs-lookup"><span data-stu-id="e3d17-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="e3d17-107">Vyřazení odstraní pouze informace organizace, zatímco úplné vymazání obnoví zařízení do továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="e3d17-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="e3d17-108">Chcete-li potvrdit, vyberte **možnost Ano.**</span><span class="sxs-lookup"><span data-stu-id="e3d17-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="e3d17-109">Dokud vymazání neskončí, stav akce Zařízení se zobrazí jako Vyřazení čeká na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="e3d17-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="e3d17-110">Po dokončení akce se mobilní zařízení v seznamu spravovaného zařízení už nebude zobrazovat.</span><span class="sxs-lookup"><span data-stu-id="e3d17-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="e3d17-111">**Poznámka:** Firemní data nelze odebrat ze zařízení, která jsou připojena k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e3d17-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="e3d17-112">Podrobné informace o účincích akcí Vyřazení a vymazání, včetně toho, co je zachováno a co se odstraní, najdete [v tématu Odebrání zařízení pomocí vymazání, vyřazení nebo ručního zrušení registrace zařízení](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="e3d17-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="e3d17-113">Pokud chcete vymazat všechna data ze zařízení s macOS, [přečtěte si přečtěte si přečtěte si tématu Vymazání všech dat ze zařízení s macOS.](https://docs.microsoft.com/intune/device-erase)</span><span class="sxs-lookup"><span data-stu-id="e3d17-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>