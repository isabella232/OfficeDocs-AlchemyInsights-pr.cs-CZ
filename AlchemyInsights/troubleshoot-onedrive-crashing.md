---
title: Poradce při potížích s havárií OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748795"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6b9e5-102">Poradce při potížích s havárií OneDrivu</span><span class="sxs-lookup"><span data-stu-id="6b9e5-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6b9e5-103">Pokud OneDrive opakovaně havaruje, vyzkoušejte tyto kroky pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="6b9e5-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6b9e5-104">**Ujistěte se, že klíče registru nejsou nastaveny:**</span><span class="sxs-lookup"><span data-stu-id="6b9e5-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6b9e5-105">Pomocí Editoru registru přejděte na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6b9e5-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6b9e5-106">Pokud disableFileSyncNGSC je k dispozici a nastavte na hodnotu 1, otevřete klíč a změňte hodnotu na 0.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6b9e5-107">Ruční spuštění OneDrivu tak, že přejdete na úvodní obrazovku</span><span class="sxs-lookup"><span data-stu-id="6b9e5-107">Manually launch OneDrive by going to Start</span></span> ![Stisknutí klávesy Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6b9e5-109">, zadejte do vyhledávacího pole OneDrive a klikněte na desktopovou aplikaci OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6b9e5-110">**Resetování OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="6b9e5-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6b9e5-111">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="6b9e5-111">Notes:</span></span>

- <span data-ttu-id="6b9e5-112">Resetováním OneDrivu odpojíte všechna stávající synchronizační připojení (včetně osobního OneDrivu, pokud je nastavený).</span><span class="sxs-lookup"><span data-stu-id="6b9e5-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6b9e5-113">O soubory ani data nedojde resetováním OneDrivu v počítači.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6b9e5-114">**Resetování OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="6b9e5-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6b9e5-115">Otevřete dialogové okno Spustit stisknutím klávesy Windows a R.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6b9e5-116">Zadejte %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stiskněte OK.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6b9e5-117">Krátce se může zobrazit okno příkazu.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6b9e5-118">Ruční spuštění OneDrivu tak, že přejdete na úvodní obrazovku</span><span class="sxs-lookup"><span data-stu-id="6b9e5-118">Manually launch OneDrive by going to Start</span></span> ![Stisknutí klávesy Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6b9e5-120">, zadejte do vyhledávacího pole OneDrive a klikněte na desktopovou aplikaci OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6b9e5-121">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="6b9e5-121">Notes:</span></span>

- <span data-ttu-id="6b9e5-122">Pokud jste se rozhodli synchronizovat pouze některé složky před resetováním, budete to muset udělat znovu po dokončení synchronizace.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6b9e5-123">Další informace [načtěte: Zvolte, které složky OneDrivu se mají synchronizovat s](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   počítačem.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6b9e5-124">Budete to muset dokončit pro osobní OneDrive a OneDrive pro firmy.</span><span class="sxs-lookup"><span data-stu-id="6b9e5-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>