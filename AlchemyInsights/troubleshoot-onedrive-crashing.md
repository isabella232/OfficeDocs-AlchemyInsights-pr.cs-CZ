---
title: Odstraňování potíží s OneDrivem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664991"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="5ba8c-102">Odstraňování potíží s OneDrivem</span><span class="sxs-lookup"><span data-stu-id="5ba8c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="5ba8c-103">Pokud se OneDrive opakovaně zhroutí, zkuste tyto kroky:</span><span class="sxs-lookup"><span data-stu-id="5ba8c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="5ba8c-104">**Zkontrolujte, jestli nejsou nastavené klíče registru:**</span><span class="sxs-lookup"><span data-stu-id="5ba8c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="5ba8c-105">Použití Editoru registru, přejděte na HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="5ba8c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="5ba8c-106">Pokud je DisableFileSyncNGSC přítomen a je nastaven na 1, otevřete klíč a změňte hodnotu na 0.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="5ba8c-107">Ruční spuštění OneDrivu tak, že přejdete na Start</span><span class="sxs-lookup"><span data-stu-id="5ba8c-107">Manually launch OneDrive by going to Start</span></span> ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="5ba8c-109">, do vyhledávacího pole zadejte OneDrive a klikněte na desktopovou aplikaci OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="5ba8c-110">**Resetování OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="5ba8c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="5ba8c-111">Komentář</span><span class="sxs-lookup"><span data-stu-id="5ba8c-111">Notes:</span></span>

- <span data-ttu-id="5ba8c-112">Obnovením OneDrivu se odpojí všechna vaše stávající synchronizovaná připojení (včetně osobního OneDrivu, pokud je nastavená).</span><span class="sxs-lookup"><span data-stu-id="5ba8c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="5ba8c-113">Obnovením OneDrivu na počítači nepřijdete o soubory ani data.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="5ba8c-114">**Obnovení OneDrivu:**</span><span class="sxs-lookup"><span data-stu-id="5ba8c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="5ba8c-115">Stisknutím kláves Windows a R otevřete dialogové okno spustit.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="5ba8c-116">Zadejte% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset a stiskněte OK.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="5ba8c-117">Krátce se zobrazí okno příkazového řádku.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="5ba8c-118">Ruční spuštění OneDrivu tak, že přejdete na Start</span><span class="sxs-lookup"><span data-stu-id="5ba8c-118">Manually launch OneDrive by going to Start</span></span> ![Stiskněte klávesu Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="5ba8c-120">, do vyhledávacího pole zadejte OneDrive a klikněte na desktopovou aplikaci OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="5ba8c-121">Komentář</span><span class="sxs-lookup"><span data-stu-id="5ba8c-121">Notes:</span></span>

- <span data-ttu-id="5ba8c-122">Pokud jste se rozhodli synchronizovat jenom některé složky před obnovením, budete se muset pokusit po dokončení synchronizace.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="5ba8c-123">Přečtěte si o [tom, které složky OneDrivu se mají synchronizovat s počítačem](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85),   kde najdete další informace.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="5ba8c-124">Tento postup musíte provést pro svůj osobní OneDrive a OneDrive pro firmy.</span><span class="sxs-lookup"><span data-stu-id="5ba8c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>