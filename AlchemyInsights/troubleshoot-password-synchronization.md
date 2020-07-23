---
title: Poradce při potížích se synchronizací hesel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387870"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="2dad4-102">Poradce při potížích se synchronizací hesel</span><span class="sxs-lookup"><span data-stu-id="2dad4-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="2dad4-103">Chcete-li vyřešit problémy se synchronizací hesel, začněte pomocí této úlohy řešení potíží služby AAD Connect a zjistěte, proč se hesla nesynchronizují.</span><span class="sxs-lookup"><span data-stu-id="2dad4-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="2dad4-104">Začněte tak, že přejdete na [Spravovat přímou synchronizaci](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="2dad4-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="2dad4-105">Otevřete novou relaci prostředí Windows PowerShell na serveru Azure AD Connect a vyberte možnost **Spustit jako správce.**</span><span class="sxs-lookup"><span data-stu-id="2dad4-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="2dad4-106">Spustit set-executionPolicy RemoteSigned nebo Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="2dad4-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="2dad4-107">Spusťte Průvodce azure ad připojení.</span><span class="sxs-lookup"><span data-stu-id="2dad4-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="2dad4-108">Přejděte na stránku Další úkoly > **Poradce při potížích s**  >  **dalšími**úkoly .</span><span class="sxs-lookup"><span data-stu-id="2dad4-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="2dad4-109">Výběrem **možnosti Spustit** otevřete nabídku řešení potíží s PowerShellem.</span><span class="sxs-lookup"><span data-stu-id="2dad4-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="2dad4-110">Vyberte **Možnost Poradce při potížích se synchronizací hesel**.</span><span class="sxs-lookup"><span data-stu-id="2dad4-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="2dad4-111">Problém je obvykle, že heslo není synchronizován pro konkrétní uživatelský účet.</span><span class="sxs-lookup"><span data-stu-id="2dad4-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="2dad4-112">**Poznámky** Synchronizace hesel se nezdaří, pokud poslední úspěšná synchronizace hesel byla před nějakým časem.</span><span class="sxs-lookup"><span data-stu-id="2dad4-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="2dad4-113">Další informace o řešení potíží se synchronizací hesel najdete [v tématu Poradce při potížích se synchronizací hash hesel se synchronizací Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="2dad4-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>