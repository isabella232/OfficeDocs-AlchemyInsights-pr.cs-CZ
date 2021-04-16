---
title: 0x8004de40 při spuštění OneDrivu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813645"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="c981a-102">0x8004de40 při spuštění OneDrivu</span><span class="sxs-lookup"><span data-stu-id="c981a-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="c981a-103">Pokud se při přihlašování **0x8004de40** OneDrivu zobrazí chybová zpráva, restartujte počítač při připojení k vaší pracovní nebo školní doméně.</span><span class="sxs-lookup"><span data-stu-id="c981a-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="c981a-104">Pokud se po restartování zobrazí tato chyba, zkuste to, když jste připojení k vaší pracovní nebo školní doméně:</span><span class="sxs-lookup"><span data-stu-id="c981a-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="c981a-105">Klikněte na Start a  do vyhledávacího pole zadejte **cmd** nebo příkazový řádek, klikněte pravým tlačítkem myši na aplikaci příkazového řádku a vyberte **Spustit jako správce**.</span><span class="sxs-lookup"><span data-stu-id="c981a-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="c981a-106">Pokud se zobrazí výzva k zadání hesla správce nebo k potvrzení, zadejte heslo nebo klikněte na **Povolit.**</span><span class="sxs-lookup"><span data-stu-id="c981a-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="c981a-107">V okně Příkazového řádku zadejte **dsregcmd /leave**  a počkejte, až se příkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="c981a-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="c981a-108">Potom zadejte **dsregcmd /join** a počkejte, až se příkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="c981a-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="c981a-109">Restartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="c981a-109">Reboot your computer.</span></span>
