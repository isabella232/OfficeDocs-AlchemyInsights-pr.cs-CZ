---
title: Nastavení clientAccessServerEnabled na Hodnotu True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523833"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="35b69-102">Nastavení clientAccessServerEnabled na Hodnotu True</span><span class="sxs-lookup"><span data-stu-id="35b69-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="35b69-103">Pokud nemůžete zašifrovanou e-mailovou zprávu otevřít a místo toho uvidíte přílohu zprávy **o** otevření, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="35b69-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="35b69-104">Připojte se k Exchange Online PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="35b69-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="35b69-105">Pokud se chcete připojit k Exchange Online PowerShellu, musíte se přihlásit pomocí účtu globálního správce nebo správce Exchange.</span><span class="sxs-lookup"><span data-stu-id="35b69-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="35b69-106">a.</span><span class="sxs-lookup"><span data-stu-id="35b69-106">a.</span></span> <span data-ttu-id="35b69-107">Otevřete Windows PowerShell a spusťte následující příkaz: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="35b69-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="35b69-108">b.</span><span class="sxs-lookup"><span data-stu-id="35b69-108">b.</span></span> <span data-ttu-id="35b69-109">V dialogovém **okně Windows PowerShell Credential Request** (Žádost o pověření windows PowerShellu) zadejte svůj pracovní nebo školní účet a heslo, c.</span><span class="sxs-lookup"><span data-stu-id="35b69-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="35b69-110">Klikněte na tlačítko **OK**.</span><span class="sxs-lookup"><span data-stu-id="35b69-110">Click **OK**.</span></span> 

2. <span data-ttu-id="35b69-111">Spuštěním následujícího příkazu vytvořte novou relaci:</span><span class="sxs-lookup"><span data-stu-id="35b69-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="35b69-112">a.</span><span class="sxs-lookup"><span data-stu-id="35b69-112">a.</span></span> <span data-ttu-id="35b69-113">Spusťte tento příkaz:</span><span class="sxs-lookup"><span data-stu-id="35b69-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="35b69-114">Příkaz `Get-IRMConfiguration` Spustit</span><span class="sxs-lookup"><span data-stu-id="35b69-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="35b69-115">Zkontrolujte nastavení **ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="35b69-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="35b69-116">a.</span><span class="sxs-lookup"><span data-stu-id="35b69-116">a.</span></span> <span data-ttu-id="35b69-117">Pokud **je nastavení ClientAccessServerEnabled** nastavené na **False,** spusťte následující rutinu: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="35b69-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="35b69-118">Relaci PowerShellu vždycky zavřete pomocí následujícího příkazu: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="35b69-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="35b69-119">Další informace najdete v článku [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="35b69-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

