---
title: Vzdálená správa zařízení Intune pomocí teamvieweru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554840"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="d2d1b-102">Vzdálená správa zařízení Intune pomocí teamvieweru</span><span class="sxs-lookup"><span data-stu-id="d2d1b-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="d2d1b-103">Zařízení spravovaná službou Intune lze spravovat vzdáleně pomocí [aplikace TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="d2d1b-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="d2d1b-104">Chcete-li spravovat Intune pomocí teamvieweru, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="d2d1b-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="d2d1b-105">Začněte získáním přihlašovacích údajů od teamvieweru a nastavte konektor TeamViewer v Intune.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="d2d1b-106">To umožňuje správci zadat přihlašovací údaje v uživatelském rozhraní konektoru TeamViewer v části Zařízení, což je jednorázová operace k vytvoření propojení mezi Intune a službou TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="d2d1b-107">**Část 1: Zahájení relace se vzdáleným zařízením**</span><span class="sxs-lookup"><span data-stu-id="d2d1b-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="d2d1b-108">V části **Všechna zařízení**vyberte zařízení, se kterým chcete spustit vzdálenou relaci.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="d2d1b-109">Od **... Další**možnost – vyberte **možnost Nová relace vzdálené pomoci**.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="d2d1b-110">Vyberte **Ano,** chcete-li potvrdit, že chcete vytvořit vzdálenou relaci.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="d2d1b-111">Po "Zahájení nové vzdálené relace" požadavek je potvrzena službou TeamViewer, uvidíte možnost **zahájit vzdálenou pomoc** v podrobnostech přehled (nebo Essentials) podokno pro zařízení.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="d2d1b-112">Výběrem **možnosti Zobrazit další** rozbalíte podokno a zobrazíte stav vzdálená pomoc.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="d2d1b-113">Chcete-li zahájit relaci na straně správce, vyberte **možnost Spustit vzdálenou relaci.**</span><span class="sxs-lookup"><span data-stu-id="d2d1b-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="d2d1b-114">Zvolte stažení binárního souboru TeamViewer (Windows) a vyberte **spustit**.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="d2d1b-115">**Poznámka:** Můžete ignorovat libovolnou stránku webového prohlížeče otevřenou na webu TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="d2d1b-116">Potvrďte požadavek, aby aplikace TeamViewer v zařízení provádět změny (pouze windows).</span><span class="sxs-lookup"><span data-stu-id="d2d1b-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="d2d1b-117">Aplikace TeamViewer se spustí a obsahuje kód relace pro ověření připojení ke vzdálenému zařízení.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="d2d1b-118">**Část 2: Na zařízení, které je cílené pro vzdálenou relaci**</span><span class="sxs-lookup"><span data-stu-id="d2d1b-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="d2d1b-119">Otevřete portál společnosti Intune.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="d2d1b-120">Vyhledejte příznak oznámení: "Správce IT požaduje řízení tohoto zařízení pro relaci vzdálené pomoci" a vyberte oznámení.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="d2d1b-121">Zvolte stažení aplikace TeamViewer nebo potvrzením stažení aplikace TeamViewer z obchodu s aplikacemi a vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="d2d1b-122">**Poznámka:** Můžete ignorovat libovolnou stránku webového prohlížeče otevřenou na webu TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="d2d1b-123">Potvrďte požadavek, aby aplikace TeamViewer v zařízení provádět změny (pouze windows).</span><span class="sxs-lookup"><span data-stu-id="d2d1b-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="d2d1b-124">Aplikace TeamViewer se spustí a obsahuje kód relace pro ověření připojení ke vzdálenému zařízení.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="d2d1b-125">Vyskakovací okno se zeptá, zda chcete povolit spuštění relace.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="d2d1b-126">**Poznámka:** Kódy relace generované službou TeamViewer jsou pouze jednorázové použití.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="d2d1b-127">Pokud připojení ztratíte, musíte:</span><span class="sxs-lookup"><span data-stu-id="d2d1b-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="d2d1b-128">Zavřete instanci aplikace TeamViewer na vzdáleném zařízení a na pracovní stanici správce.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="d2d1b-129">Zavřete portál společnosti na vzdáleném zařízení.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="d2d1b-130">Spusťte novou "Novou relaci vzdálené pomoci" z portálu pro správu.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="d2d1b-131">Znovu otevřete portál společnosti na vzdáleném zařízení a obdržíte nové oznámení.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="d2d1b-132">Stáhněte a otevřete aplikaci TeamViewer na vzdáleném zařízení i na pracovní stanici správce, jako dříve.</span><span class="sxs-lookup"><span data-stu-id="d2d1b-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>