---
title: Odebrání dat a utírání zařízení z Intune
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416306"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="bcd7f-102">Odebrání dat a utírání zařízení z Intune</span><span class="sxs-lookup"><span data-stu-id="bcd7f-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="bcd7f-103">Pomocí vzdálených akcí Vyřazení zařízení a Vymazání zařízení můžete odebrat data společnosti spravovaných Intune nebo obnovit tovární nastavení a vrátit zařízení do výchozího nastavení.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="bcd7f-104">Přihlaste se ke Správě zařízení Microsoft 365 a přejděte na **Zařízení**  >  **všechna zařízení.**</span><span class="sxs-lookup"><span data-stu-id="bcd7f-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="bcd7f-105">Vyberte zařízení, které chcete vymazat.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="bcd7f-106">Vyberte typ vzdáleného vymazání, které chcete udělat.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="bcd7f-107">Vyřazení odstraní jenom informace organizace, zatímco úplné vymazání obnoví zařízení do továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="bcd7f-108">Výběrem **možnosti Ano** potvrďte.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="bcd7f-109">Dokud se vymazání nedokončí, zobrazí se stav akce Zařízení jako Čeká na *vyřazení.*</span><span class="sxs-lookup"><span data-stu-id="bcd7f-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="bcd7f-110">Po dokončení akce se už mobilní zařízení v seznamu spravovaného zařízení nebude zobrazit.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="bcd7f-111">Ze zařízení PŘIPOJENÝch k Azure AD nelze odebrat data společnosti.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="bcd7f-112">Úplné podrobnosti o efektu akcí Vyřazení a vymazání, včetně toho, co se zachová a co se odstraní, najdete v následující dokumentaci:</span><span class="sxs-lookup"><span data-stu-id="bcd7f-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="bcd7f-113">[Zařízení odeberte vymazáním, vyřazením nebo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)ručním zrušení registrace zařízení.</span><span class="sxs-lookup"><span data-stu-id="bcd7f-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="bcd7f-114">Jak vymazat jenom podniková data z aplikací spravovaných přes Intune</span><span class="sxs-lookup"><span data-stu-id="bcd7f-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="bcd7f-115">[Vymažte všechna data ze zařízení s macOS.](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)</span><span class="sxs-lookup"><span data-stu-id="bcd7f-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>