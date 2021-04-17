---
title: Poradce při potížích s chybou OneDrivu
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826192"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="7ab56-102">Poradce při potížích s chybou OneDrivu</span><span class="sxs-lookup"><span data-stu-id="7ab56-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="7ab56-103">Pokud onedrive opakovaně dochází k chybě, zkuste tento postup řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="7ab56-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="7ab56-104">**Ujistěte se, že nejsou nastavené klíče registru:**</span><span class="sxs-lookup"><span data-stu-id="7ab56-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="7ab56-105">Pomocí Editoru registru přejděte na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="7ab56-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="7ab56-106">Pokud je funkce DisableFileSyncNGSC k dispozici a je nastavená na hodnotu 1, otevřete klávesu a změňte hodnotu na 0.</span><span class="sxs-lookup"><span data-stu-id="7ab56-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="7ab56-107">Ruční spuštění OneDrivu tak, že půjdete na Start</span><span class="sxs-lookup"><span data-stu-id="7ab56-107">Manually launch OneDrive by going to Start</span></span> ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="7ab56-109">, do vyhledávacího pole zadejte OneDrive a klikněte na desktopové aplikaci OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7ab56-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="7ab56-110">**Resetování OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="7ab56-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="7ab56-111">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="7ab56-111">Notes:</span></span>

- <span data-ttu-id="7ab56-112">Resetováním OneDrivu se odpojí všechna stávající synchronizační připojení (včetně osobního OneDrivu při nastavení).</span><span class="sxs-lookup"><span data-stu-id="7ab56-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="7ab56-113">Soubory ani data neztratíte resetováním OneDrivu na počítači.</span><span class="sxs-lookup"><span data-stu-id="7ab56-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="7ab56-114">**Resetování OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="7ab56-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="7ab56-115">Otevřete dialogové okno Spustit stisknutím klávesy Windows a klávesy R.</span><span class="sxs-lookup"><span data-stu-id="7ab56-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="7ab56-116">Zadejte %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stiskněte OK.</span><span class="sxs-lookup"><span data-stu-id="7ab56-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="7ab56-117">Může se krátce zobrazit příkazové okno.</span><span class="sxs-lookup"><span data-stu-id="7ab56-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="7ab56-118">Ruční spuštění OneDrivu tak, že půjdete na Start</span><span class="sxs-lookup"><span data-stu-id="7ab56-118">Manually launch OneDrive by going to Start</span></span> ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="7ab56-120">, do vyhledávacího pole zadejte OneDrive a klikněte na desktopové aplikaci OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7ab56-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="7ab56-121">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="7ab56-121">Notes:</span></span>

- <span data-ttu-id="7ab56-122">Pokud jste se rozhodli synchronizovat jenom některé složky před obnovením továrního nastavení, budete to muset udělat znovu po dokončení synchronizace.</span><span class="sxs-lookup"><span data-stu-id="7ab56-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="7ab56-123">Přečtěte [si informace o tom, které složky OneDrivu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)se mají synchronizovat s   počítačem.</span><span class="sxs-lookup"><span data-stu-id="7ab56-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="7ab56-124">Tento proces budete muset dokončit pro svůj osobní OneDrive a OneDrive pro firmy.</span><span class="sxs-lookup"><span data-stu-id="7ab56-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>