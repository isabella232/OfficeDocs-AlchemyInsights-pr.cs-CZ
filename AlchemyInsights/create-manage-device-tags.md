---
title: Vytváření a správa značek nebo skupin zařízení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731341"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="adfec-102">Vytváření a správa značek nebo skupin zařízení</span><span class="sxs-lookup"><span data-stu-id="adfec-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="adfec-103">Přidáním značek na zařízeních vytvoříte logickou skupinu.</span><span class="sxs-lookup"><span data-stu-id="adfec-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="adfec-104">Značky zařízení podporují správné mapování sítě, což umožňuje připojit různé značky k zachycení kontextu a povolit vytváření dynamických seznamu jako součást incidentu.</span><span class="sxs-lookup"><span data-stu-id="adfec-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="adfec-105">Značky můžete použít jako filtr v zobrazení seznamu Zařízení nebo pro seskupit zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="adfec-106">Další informace o seskupování zařízení najdete v tématu [Vytvoření a správa značek zařízení](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="adfec-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="adfec-107">Značky na zařízeních můžete přidat pomocí:</span><span class="sxs-lookup"><span data-stu-id="adfec-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="adfec-108">Používání portálu</span><span class="sxs-lookup"><span data-stu-id="adfec-108">Using the portal</span></span>

- <span data-ttu-id="adfec-109">Nastavení hodnoty klíče registru</span><span class="sxs-lookup"><span data-stu-id="adfec-109">Setting a registry key value</span></span>
 
<span data-ttu-id="adfec-110">**Poznámka:** Mezi přidáním značky na zařízení a jeho dostupností v seznamu zařízení a na stránce zařízení může být latence.</span><span class="sxs-lookup"><span data-stu-id="adfec-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="adfec-111">Pokud chcete přidat značky zařízení pomocí rozhraní API, podívejte se na téma [Přidání nebo odebrání značek zařízení API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="adfec-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="adfec-112">Přidání a správa značek zařízení pomocí portálu</span><span class="sxs-lookup"><span data-stu-id="adfec-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="adfec-113">Vyberte zařízení, na které chcete spravovat značky.</span><span class="sxs-lookup"><span data-stu-id="adfec-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="adfec-114">Zařízení můžete vybrat nebo vyhledat v libovolném z následujících zobrazení:</span><span class="sxs-lookup"><span data-stu-id="adfec-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="adfec-115">**Řídicí panel operací zabezpečení** V části Top devices with active alerts (Nejlepší zařízení s aktivními výstrahami) vyberte název zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="adfec-116">**Fronta upozornění** : V frontě upozornění vyberte název zařízení vedle ikony zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="adfec-117">**Seznam zařízení** – v seznamu zařízení vyberte název zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="adfec-118">**Vyhledávací pole** : V rozevírací nabídce vyberte Zařízení a zadejte název zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="adfec-119">Můžete se taky dostat na stránku s upozorněním prostřednictvím zobrazení souborů a IP adres.</span><span class="sxs-lookup"><span data-stu-id="adfec-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="adfec-120">Na **řádku akcí** Odpovědi vyberte Spravovat značky.</span><span class="sxs-lookup"><span data-stu-id="adfec-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="adfec-121">Pokud chcete najít nebo vytvořit značky, zadejte ho.</span><span class="sxs-lookup"><span data-stu-id="adfec-121">Type to find or create tags.</span></span>

<span data-ttu-id="adfec-122">Značky se přidávají do zobrazení zařízení a projeví se v zobrazení seznamu Zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="adfec-123">Pak můžete pomocí filtru Značky zobrazit příslušný seznam zařízení.</span><span class="sxs-lookup"><span data-stu-id="adfec-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="adfec-124">Další informace najdete v tématu [Vytvoření a správa značek zařízení](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="adfec-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>