---
title: Nahrávání hovorů 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702083"
---
# <a name="11-call-recording"></a><span data-ttu-id="f3fcf-102">Nahrávání hovorů 1:1</span><span class="sxs-lookup"><span data-stu-id="f3fcf-102">1:1 call recording</span></span>

<span data-ttu-id="f3fcf-103">Pokud je **tlačítko Spustit záznam** v hovoru 1:1 šedé, musíte změnit nastavení zásad pro ovlivněné uživatele.</span><span class="sxs-lookup"><span data-stu-id="f3fcf-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="f3fcf-104">Pokud chcete zkontrolovat nastavení zásad, spusťte diagnostiku pro ovlivněné uživatele tak, že napíšete **Diag: Teams 1:1 Nahrávání hovorů** výše.</span><span class="sxs-lookup"><span data-stu-id="f3fcf-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="f3fcf-105">Od 31. května 2021 začneme vynucovat novou Teams hovory *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="f3fcf-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="f3fcf-106">Před touto změnou je záznam hovoru 1:1 řízený zásadou *AllowCloudRecording* Teams schůzek.</span><span class="sxs-lookup"><span data-stu-id="f3fcf-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="f3fcf-107">Tato změna je zdokumentována v příspěvku Centra zpráv: [(aktualizováno) 1:1 Úvod](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)zásad nahrávání hovorů .</span><span class="sxs-lookup"><span data-stu-id="f3fcf-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="f3fcf-108">*AllowCloudRecordingForCalls*   Možnost zásady volání je ve **$False** nastavená.</span><span class="sxs-lookup"><span data-stu-id="f3fcf-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="f3fcf-109">Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, nemusíte nic udělat.</span><span class="sxs-lookup"><span data-stu-id="f3fcf-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="f3fcf-110">Pokud chcete povolit nahrávání hovorů pro všechny uživatele v hovoru 1:1, [Teams PowerShell](/microsoftteams/teams-powershell-install) spustit následující rutinu:</span><span class="sxs-lookup"><span data-stu-id="f3fcf-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="f3fcf-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="f3fcf-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="f3fcf-112">Můžete také vytvořit novou zásadu a nastavit **možnost -AllowCloudRecordingForCalls** tak, aby $true a přiřazovat je uživatelům. </span><span class="sxs-lookup"><span data-stu-id="f3fcf-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="f3fcf-113">Další informace najdete v článku 1:1 Ovládací prvky zásad nahrávání hovorů [jsou (téměř!) Tady](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="f3fcf-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
