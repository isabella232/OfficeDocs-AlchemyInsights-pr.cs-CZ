---
title: Chyby při synchronizaci automatické registrace zařízení Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448915"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="8d371-102">Chyby při synchronizaci automatické registrace zařízení Apple</span><span class="sxs-lookup"><span data-stu-id="8d371-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="8d371-103">"Zjistili jsme, že máte jeden nebo víc tokenů ADE/DEP, které jsou v chybovém stavu.</span><span class="sxs-lookup"><span data-stu-id="8d371-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="8d371-104">Dokud se problém nevyřeší u každého ovlivněného tokenu, nebude funkce ADE fungovat podle očekávání."</span><span class="sxs-lookup"><span data-stu-id="8d371-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="8d371-105">Tato chyba se může projevit několika způsoby, mezi které patří:</span><span class="sxs-lookup"><span data-stu-id="8d371-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="8d371-106">Zařízení se nemusí synchronizovat z ABM/ASM do Intune</span><span class="sxs-lookup"><span data-stu-id="8d371-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="8d371-107">Zadání v profilu prováděcí smlouvy nemusí být neúspěšná</span><span class="sxs-lookup"><span data-stu-id="8d371-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="8d371-108">Zařízení nemusí úspěšně dokončovat registraci ADE.</span><span class="sxs-lookup"><span data-stu-id="8d371-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="8d371-109">Zkontrolujte, že v konzole Intune nehlásila chyba synchronizace v části **Zařízení > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span><span class="sxs-lookup"><span data-stu-id="8d371-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="8d371-110">Jednou z nejčastějších příčin chyby synchronizace je vypršení platnosti aktuálního tokenu.</span><span class="sxs-lookup"><span data-stu-id="8d371-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="8d371-111">V mnoha případech se problém vyřeší obnovením ovlivněného tokenu.</span><span class="sxs-lookup"><span data-stu-id="8d371-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="8d371-112">Pokud vypršela platnost jednoho nebo více vašich tokenů, podívejte se do následující dokumentace, abyste si je podle potřeby pomohli obnovit:</span><span class="sxs-lookup"><span data-stu-id="8d371-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="8d371-113">Prodloužení automatického registračního tokenu zařízení</span><span class="sxs-lookup"><span data-stu-id="8d371-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="8d371-114">Kromě toho si můžete zobrazit následující dokumentaci, abyste se mohli podívat na možná řešení jiných chyb, které způsobují chyby synchronizace tokenů:</span><span class="sxs-lookup"><span data-stu-id="8d371-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="8d371-115">Chyby synchronizace ABM/ASM pro iOS/iPadOS a macOS automated device enrollment tokens</span><span class="sxs-lookup"><span data-stu-id="8d371-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="8d371-116">Chyby synchronizace ABM/ASM pro iOS/iPadOS a macOS automated device enrollment tokens</span><span class="sxs-lookup"><span data-stu-id="8d371-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
