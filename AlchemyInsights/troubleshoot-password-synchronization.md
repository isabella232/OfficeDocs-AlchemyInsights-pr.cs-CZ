---
title: Řešení potíží s synchronizací hesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664919"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="dabe9-102">Řešení potíží s synchronizací hesel</span><span class="sxs-lookup"><span data-stu-id="dabe9-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="dabe9-103">Chcete-li vyřešit problémy se synchronizací hesel, začněte pomocí tohoto úkolu AAD Connect pro řešení potíží zjistit, proč se hesla nesynchronizují.</span><span class="sxs-lookup"><span data-stu-id="dabe9-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="dabe9-104">Začněte tím, že přejdete na [Správa přímé synchronizace](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="dabe9-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="dabe9-105">Na serveru Azure AD Connect otevřete novou relaci Windows PowerShellu a vyberte možnost **Spustit jako správce** .</span><span class="sxs-lookup"><span data-stu-id="dabe9-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="dabe9-106">Spusťte Set-ExecutionPolicy RemoteSigned nebo Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="dabe9-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="dabe9-107">Spusťte Průvodce Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="dabe9-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="dabe9-108">Přejděte na stránku další úkoly > **řešení potíží**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="dabe9-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="dabe9-109">Výběrem možnosti **Spustit** otevřete nabídku odstraňování potíží PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="dabe9-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="dabe9-110">Vyberte **Poradce při potížích s synchronizací hesel**.</span><span class="sxs-lookup"><span data-stu-id="dabe9-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="dabe9-111">Problém se obvykle nesynchronizuje s heslem pro konkrétní uživatelský účet.</span><span class="sxs-lookup"><span data-stu-id="dabe9-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="dabe9-112">**Poznámky** Synchronizace hesel se nezdaří, pokud uplynula Poslední úspěšná synchronizace hesla.</span><span class="sxs-lookup"><span data-stu-id="dabe9-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="dabe9-113">Další nápovědu k řešení potíží s synchronizací hesel najdete v článku [Poradce při synchronizaci hash synchronizace s heslem pomocí synchronizace Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="dabe9-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>