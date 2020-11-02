---
title: Chyba 0x8004de40 při spouštění OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823015"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="71921-102">Chyba 0x8004de40 při spouštění OneDrivu</span><span class="sxs-lookup"><span data-stu-id="71921-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="71921-103">Pokud se při přihlašování k OneDrivu zobrazí chybová zpráva **0x8004de40** , restartujte počítač, když jste připojení k vaší pracovní nebo školní doméně.</span><span class="sxs-lookup"><span data-stu-id="71921-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="71921-104">Pokud se tato chyba zobrazí po restartování počítače, vyzkoušejte to, co se připojuje k vaší pracovní nebo školní doméně:</span><span class="sxs-lookup"><span data-stu-id="71921-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="71921-105">Klikněte na Start a do vyhledávacího pole zadejte **cmd** nebo **Command Prompt**  , klikněte pravým tlačítkem na aplikaci příkazového řádku a vyberte  **Spustit jako správce** .</span><span class="sxs-lookup"><span data-stu-id="71921-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="71921-106">Pokud se zobrazí výzva k zadání hesla správce nebo potvrzení, zadejte heslo nebo klikněte na **Povolit** .</span><span class="sxs-lookup"><span data-stu-id="71921-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="71921-107">V okně příkazového řádku zadejte **dsregcmd/Leave**  a počkejte, až se příkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="71921-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="71921-108">Potom zadejte **dsregcmd/JOIN** a počkejte, až se příkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="71921-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="71921-109">Restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="71921-109">Reboot your computer.</span></span>
