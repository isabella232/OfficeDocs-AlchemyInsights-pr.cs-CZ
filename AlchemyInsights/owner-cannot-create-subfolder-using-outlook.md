---
title: Vlastník nemůže vytvořit podsložku pomocí Outlooku.
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665711"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="22c91-102">Vlastník nemůže vytvořit podsložku pomocí Outlooku.</span><span class="sxs-lookup"><span data-stu-id="22c91-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="22c91-103">**U vlastníků veřejných složek se při vytváření podsložek používá Outlook. Problém bude brzy opraven.**</span><span class="sxs-lookup"><span data-stu-id="22c91-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="22c91-104">Dále použijte jedno z následujících řešení:</span><span class="sxs-lookup"><span data-stu-id="22c91-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="22c91-105">Vytvoření podsložky pomocí Outlooku pro MAC jenom Outlook pro desktopová okna (všechny verze)</span><span class="sxs-lookup"><span data-stu-id="22c91-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="22c91-106">Vytvoření podsložky pomocí Správce EXO Shell nebo EAC</span><span class="sxs-lookup"><span data-stu-id="22c91-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="22c91-107">Změnit DefaultPublicFolderMailbox/EffectivePublicFolderMailbox u uživatele na jinou poštovní schránku, než je poštovní schránka pro složku, která způsobuje chybu</span><span class="sxs-lookup"><span data-stu-id="22c91-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="22c91-108">*Set-Mailbox user1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="22c91-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="22c91-109">Počkat na hodinu, restartovat klienta Outlooku</span><span class="sxs-lookup"><span data-stu-id="22c91-109">Wait for an hour, restart outlook client</span></span>