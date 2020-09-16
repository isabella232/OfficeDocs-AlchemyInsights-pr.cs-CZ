---
title: Oprava chyby 0x8004de40 na OneDrivu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745123"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="e562a-102">Oprava chyby 0x8004de40 na OneDrivu</span><span class="sxs-lookup"><span data-stu-id="e562a-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="e562a-103">Pokud se na OneDrivu zobrazí chyba 0x8004de40:</span><span class="sxs-lookup"><span data-stu-id="e562a-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="e562a-104">Restartujte počítač, který je připojený k doméně adresáře Acitve.</span><span class="sxs-lookup"><span data-stu-id="e562a-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="e562a-105">Pokud se restartováním problém nevyřeší, odpojte se do zařízení z Azure AD a připojte se znovu.</span><span class="sxs-lookup"><span data-stu-id="e562a-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="e562a-106">**Poznámka**: při provádění těchto kroků byste měli být v podnikové síti.</span><span class="sxs-lookup"><span data-stu-id="e562a-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="e562a-107">Tyto kroky neprovádějte, pokud se nemůžete připojit k podnikové infrastruktuře (například při cestování).</span><span class="sxs-lookup"><span data-stu-id="e562a-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="e562a-108">Otevřete příkazový řádek se zvýšenými oprávněními.</span><span class="sxs-lookup"><span data-stu-id="e562a-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="e562a-109">Pokud chcete otevřít příkazový řádek se zvýšenými oprávněními, klikněte na **Start**, pravým tlačítkem myši klikněte na **příkazový řádek**a potom klikněte na **Spustit jako správce**.</span><span class="sxs-lookup"><span data-stu-id="e562a-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="e562a-110">Zadejte *dsregcmd/Leave* a stiskněte **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="e562a-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="e562a-111">Po dokončení zadejte *dsregcmd/JOIN* a stiskněte **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="e562a-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="e562a-112">Po dokončení zavřete příkazový řádek.</span><span class="sxs-lookup"><span data-stu-id="e562a-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="e562a-113">Restartujte počítač a přihlaste se k OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="e562a-113">Reboot the computer, and log into OneDrive.</span></span>