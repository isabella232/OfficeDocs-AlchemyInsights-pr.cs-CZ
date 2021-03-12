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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733842"
---
# <a name="11-call-recording"></a><span data-ttu-id="420d8-102">Nahrávání hovorů 1:1</span><span class="sxs-lookup"><span data-stu-id="420d8-102">1:1 call recording</span></span>

<span data-ttu-id="420d8-103">Správci teď musí provést akci, aby uživatelé mohli nahrávat hovory 1:1.</span><span class="sxs-lookup"><span data-stu-id="420d8-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="420d8-104">Od 12. dubna 2021 začneme vynucovat novou možnost Zásad volání do Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="420d8-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="420d8-105">V současné době jsou možnosti nahrávání hovorů 1:1 řízeny možností *AllowCloudRecording* v zásadách schůzek v Teams.</span><span class="sxs-lookup"><span data-stu-id="420d8-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="420d8-106">Pokud mají vaši uživatelé povoleno zaznamenávat schůzky v Teams, 1:1 hovory 1:1.</span><span class="sxs-lookup"><span data-stu-id="420d8-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="420d8-107">Pokud chcete všem uživatelům blokovat nahrávání hovorů 1:1, není nutné nic dělat.</span><span class="sxs-lookup"><span data-stu-id="420d8-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="420d8-108">*Možnost zásady volání AllowCloudRecordingForCalls* se $False ve výchozím nastavení.</span><span class="sxs-lookup"><span data-stu-id="420d8-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="420d8-109">Tato změna je zdokumentovaná v následujícím příspěvku Centra zpráv: [(aktualizováno) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Úvod k zásadám nahrávání hovorů Pokud chcete nastavit možnost zásad volání teams, musíte [použít Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="420d8-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="420d8-110">**Povolení nahrávání hovorů v 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="420d8-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="420d8-111">**Zakázání nahrávání hovorů v hovorech 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="420d8-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

