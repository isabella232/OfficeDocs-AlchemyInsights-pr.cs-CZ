---
title: Nápověda k nastavení zobrazení nočního osvětlení
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404266"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="06388-102">Nápověda k nastavení zobrazení nočního osvětlení</span><span class="sxs-lookup"><span data-stu-id="06388-102">Help with the night light display setting</span></span>

<span data-ttu-id="06388-103">Další informace o nastavení zobrazení v noční době najdete v tématu Nastavení zobrazení pro [noční dobu ve Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="06388-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="06388-104">Pokud jsou možnosti nočního osvětlení v Nastavení šedé, zkontrolujte ovladač zobrazení:</span><span class="sxs-lookup"><span data-stu-id="06388-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="06388-105">Klikněte na vyhledávací pole na hlavním panelu a  zadejte **Správce zařízení** a ve výsledcích hledání vyberte Správce zařízení.</span><span class="sxs-lookup"><span data-stu-id="06388-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="06388-106">Rozbalte **položku Grafické adaptéry**.</span><span class="sxs-lookup"><span data-stu-id="06388-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="06388-107">Funkce nočního osvětlení bohužel není dostupná, pokud vaše zařízení používá ovladač DisplayLink nebo ovladač Základní displej.</span><span class="sxs-lookup"><span data-stu-id="06388-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="06388-108">Funkce nočního osvětlení používá nedávnou grafickou technologii, takže možná budete muset aktualizovat ovladač obrazovky:</span><span class="sxs-lookup"><span data-stu-id="06388-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="06388-109">Aktualizace můžete zkontrolovat tak, že v části **Spustit** aktualizaci  >    >  **nastavení & Windows**  >  **Update**  >  **vyhledat aktualizace**.</span><span class="sxs-lookup"><span data-stu-id="06388-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="06388-110">NEBO</span><span class="sxs-lookup"><span data-stu-id="06388-110">OR</span></span>

- <span data-ttu-id="06388-111">Pokud chcete ručně stáhnout a nainstalovat nejnovější ovladače zobrazení, navštivte web podpory výrobce hardwaru.</span><span class="sxs-lookup"><span data-stu-id="06388-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="06388-112">Resetování nočního osvětlení v registru</span><span class="sxs-lookup"><span data-stu-id="06388-112">Reset night light in the registry</span></span>

<span data-ttu-id="06388-113">Pokud aktualizace ovladače displeje nefunguje, bude možná potřeba obnovit noční osvětlení v registru.</span><span class="sxs-lookup"><span data-stu-id="06388-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="06388-114">**Upozornění:** Tento krok řešení potíží se doporučuje jenom pro pokročilé uživatele.</span><span class="sxs-lookup"><span data-stu-id="06388-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="06388-115">Pokud registr změníte nesprávně, může dojít k vážným problémům.</span><span class="sxs-lookup"><span data-stu-id="06388-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="06388-116">Pokud chcete přidat ochranu, zálohujte registr před jeho úpravami, abyste ho mohli obnovit, pokud dojde k problémům.</span><span class="sxs-lookup"><span data-stu-id="06388-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="06388-117">Do vyhledávacího pole zadejte **regedit** a ve výsledcích hledání vyberte **Editor** registru.</span><span class="sxs-lookup"><span data-stu-id="06388-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="06388-118">Přejděte na následující klíč registru:</span><span class="sxs-lookup"><span data-stu-id="06388-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="06388-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="06388-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="06388-120">Export a odstranění následujícího podklíče:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="06388-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="06388-121">Export a odstranění následujícího podklíče:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="06388-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="06388-122">Restartujte Windows a ověřte, jestli jsou dostupné možnosti nočního osvětlení.</span><span class="sxs-lookup"><span data-stu-id="06388-122">Restart Windows and verify if the night light options are available.</span></span>


