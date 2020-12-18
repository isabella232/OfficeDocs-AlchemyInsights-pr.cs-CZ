---
title: Chyby synchronizace automatického zápisu zařízení Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714690"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="d9bda-102">Chyby synchronizace automatického zápisu zařízení Apple</span><span class="sxs-lookup"><span data-stu-id="d9bda-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="d9bda-103">Zjistili jsme, že máte jeden nebo víc tokenů ADE/DEP, které jsou v chybovém stavu.</span><span class="sxs-lookup"><span data-stu-id="d9bda-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="d9bda-104">Dokud nebude chybový stav vyřešen u každého úspěšného tokenu, nebudou funkce ADE fungovat stejně.</span><span class="sxs-lookup"><span data-stu-id="d9bda-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="d9bda-105">Tato chyba může být v mnoha ohledech:</span><span class="sxs-lookup"><span data-stu-id="d9bda-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="d9bda-106">Zařízení se nemusí synchronizovat z ABM/ASM na Intune</span><span class="sxs-lookup"><span data-stu-id="d9bda-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="d9bda-107">Přiřazení profilu registrace se nemusí zdařit</span><span class="sxs-lookup"><span data-stu-id="d9bda-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="d9bda-108">Zařízení nemusí dokončit zápis ADE.</span><span class="sxs-lookup"><span data-stu-id="d9bda-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="d9bda-109">Zkontrolujte, jestli je chyba synchronizace hlášená v konzoli Intune v části **zařízení > zaregistrovat zařízení > tokeny programu Apple enrollment > pro zápis** , a podívejte se na následující dokumentaci, kde se zobrazí jakákoli potenciální Oprava:</span><span class="sxs-lookup"><span data-stu-id="d9bda-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="d9bda-110">Chyby synchronizace ABM/ASM pro tokeny automatických zápisů s iOS/iPadOS a macOS</span><span class="sxs-lookup"><span data-stu-id="d9bda-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
