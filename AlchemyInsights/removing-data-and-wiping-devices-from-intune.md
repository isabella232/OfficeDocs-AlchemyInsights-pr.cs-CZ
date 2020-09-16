---
title: Odebrání dat a vymazání zařízení z Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701276"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="b409a-102">Odebrání dat a vymazání zařízení z Intune</span><span class="sxs-lookup"><span data-stu-id="b409a-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="b409a-103">Odřazení zařízení a vymazání zařízení: vzdálené akce mohou být použity k odebrání dat společnosti spravovaných intunem nebo k provedení továrního resetu a obnovení výchozího nastavení zařízení.</span><span class="sxs-lookup"><span data-stu-id="b409a-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="b409a-104">Přihlaste se ke správě zařízení Microsoft 365 a **přejděte na**  >  **všechna zařízení**.</span><span class="sxs-lookup"><span data-stu-id="b409a-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="b409a-105">Vyberte zařízení, které chcete vymazat.</span><span class="sxs-lookup"><span data-stu-id="b409a-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="b409a-106">Vyberte typ vzdáleného vymazání, které chcete provést.</span><span class="sxs-lookup"><span data-stu-id="b409a-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="b409a-107">Možnost vyřazení odstraní jenom informace o organizaci, zatímco možnost úplné vymazání zařízení obnoví do továrního nastavení.</span><span class="sxs-lookup"><span data-stu-id="b409a-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="b409a-108">Kliknutím na **Ano** potvrďte.</span><span class="sxs-lookup"><span data-stu-id="b409a-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="b409a-109">Až do doby vymazání skončí, zobrazí se stav akce zařízení jako čekající vyřazení.</span><span class="sxs-lookup"><span data-stu-id="b409a-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="b409a-110">Po dokončení akce se v seznamu spravovaných zařízení už nezobrazuje mobilní zařízení.</span><span class="sxs-lookup"><span data-stu-id="b409a-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="b409a-111">**Poznámka:** Data společnosti nejde odebrat ze zařízení připojených k Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b409a-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="b409a-112">Podrobné informace o vlivu akcí vyřazení a vymazání, včetně informací o tom, co je zachováno a o odstranění, najdete v tématu [odebrání zařízení pomocí vymazání, vyřazení nebo ručním odregistraci zařízení](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="b409a-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="b409a-113">Pokud chcete vymazat všechna data ze zařízení macOS, přečtěte si článek [vymazání všech dat ze zařízení MacOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="b409a-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>