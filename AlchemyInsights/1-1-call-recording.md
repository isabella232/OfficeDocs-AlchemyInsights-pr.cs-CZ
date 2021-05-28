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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696915"
---
# <a name="11-call-recording"></a><span data-ttu-id="b3fc4-102">Nahrávání hovorů 1:1</span><span class="sxs-lookup"><span data-stu-id="b3fc4-102">1:1 call recording</span></span>

<span data-ttu-id="b3fc4-103">Pokud je **tlačítko Spustit záznam** v hovoru 1:1 šedé, musíte změnit nastavení zásad pro ovlivněné uživatele.</span><span class="sxs-lookup"><span data-stu-id="b3fc4-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="b3fc4-104">Od 31. května 2021 začneme vynucovat novou Teams hovory *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="b3fc4-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="b3fc4-105">Před touto změnou je záznam hovoru 1:1 řízený zásadou *AllowCloudRecording* Teams schůzek.</span><span class="sxs-lookup"><span data-stu-id="b3fc4-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="b3fc4-106">Tato změna je zdokumentována v příspěvku Centra zpráv: [(aktualizováno) 1:1 Úvod](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)zásad nahrávání hovorů .</span><span class="sxs-lookup"><span data-stu-id="b3fc4-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="b3fc4-107">*AllowCloudRecordingForCalls*   Možnost zásady volání je ve **$False** nastavená.</span><span class="sxs-lookup"><span data-stu-id="b3fc4-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="b3fc4-108">Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, nemusíte nic udělat.</span><span class="sxs-lookup"><span data-stu-id="b3fc4-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="b3fc4-109">Pokud chcete povolit nahrávání hovorů pro všechny uživatele v hovoru 1:1, Teams PowerShellu spustit následující rutinu:</span><span class="sxs-lookup"><span data-stu-id="b3fc4-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="b3fc4-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="b3fc4-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="b3fc4-111">Můžete také vytvořit novou zásadu a nastavit **možnost -AllowCloudRecordingForCalls** tak, aby $true a přiřazovat je uživatelům. </span><span class="sxs-lookup"><span data-stu-id="b3fc4-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="b3fc4-112">Další informace najdete v článku 1:1 Ovládací prvky zásad nahrávání hovorů [jsou (téměř!) Tady](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="b3fc4-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
