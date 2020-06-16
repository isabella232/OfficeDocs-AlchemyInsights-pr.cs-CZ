---
title: Vlastník nemůže vytvořit podsložky pomocí aplikace Outlook.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748789"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="b34f5-102">Vlastník nemůže vytvořit podsložky pomocí aplikace Outlook.</span><span class="sxs-lookup"><span data-stu-id="b34f5-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="b34f5-103">**Probíhá problém s vlastníky veřejných složek, kteří vytvářejí podsložky pomocí aplikace Outlook. Problém bude brzy vyřešen.**</span><span class="sxs-lookup"><span data-stu-id="b34f5-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="b34f5-104">Mezitím použijte jedno z následujících řešení:</span><span class="sxs-lookup"><span data-stu-id="b34f5-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="b34f5-105">Použití Outlooku pro MAC k vytvoření podsložky, protože problém má vliv pouze na okna Outlooku pro stolní počítače (všechny verze).</span><span class="sxs-lookup"><span data-stu-id="b34f5-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="b34f5-106">Mít admin vytvořit podsložku pomocí EXO Shell nebo EAC</span><span class="sxs-lookup"><span data-stu-id="b34f5-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="b34f5-107">Změna defaultpublicFolderMailbox/EffectivePublicFolderMailbox na uživatele na jinou poštovní schránku než poštovní schránku obsahu pro složku, která způsobuje potíže</span><span class="sxs-lookup"><span data-stu-id="b34f5-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="b34f5-108">*Výchozí výchozí poštovní schránka Poštovní složkyMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="b34f5-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="b34f5-109">Počkejte hodinu, restartujte klienta outlooku</span><span class="sxs-lookup"><span data-stu-id="b34f5-109">Wait for an hour, restart outlook client</span></span>