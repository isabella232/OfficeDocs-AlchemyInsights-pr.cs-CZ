---
title: Vlastník nemůže vytvořit podsadu pomocí Outlooku.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836128"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="d0ff6-102">Vlastník nemůže vytvořit podsadu pomocí Outlooku.</span><span class="sxs-lookup"><span data-stu-id="d0ff6-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="d0ff6-103">**Při vytváření podsložek pomocí Outlooku dochází k probíhajícímu problému s vlastníky veřejných složek. Problém bude brzy opravený.**</span><span class="sxs-lookup"><span data-stu-id="d0ff6-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="d0ff6-104">Mezitím použijte jedno z následujících alternativních řešení:</span><span class="sxs-lookup"><span data-stu-id="d0ff6-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="d0ff6-105">Vytvoření podsložky v Outlooku pro MAC se týká jenom Outlooku pro desktopová okna (všechny verze).</span><span class="sxs-lookup"><span data-stu-id="d0ff6-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="d0ff6-106">Vytvoření podsložky správcem pomocí prostředí EXO Shell nebo EAC</span><span class="sxs-lookup"><span data-stu-id="d0ff6-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="d0ff6-107">Změna DefaultPublicFolderMailbox/EffectivePublicFolderMailbox u uživatele na jinou poštovní schránku než poštovní schránku obsahu pro složku způsobující problém</span><span class="sxs-lookup"><span data-stu-id="d0ff6-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="d0ff6-108">*Set-Mailbox User1 DefaultPublikaceMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="d0ff6-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="d0ff6-109">Počkejte hodinu, restartujte klienta Outlooku.</span><span class="sxs-lookup"><span data-stu-id="d0ff6-109">Wait for an hour, restart outlook client</span></span>