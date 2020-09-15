---
title: Chyba 4c7 v Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700196"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="c5327-102">Chyba 4c7 v Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c5327-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="c5327-103">K této chybě dochází, protože Microsoft Teams vyžaduje ověřování formulářů.</span><span class="sxs-lookup"><span data-stu-id="c5327-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="c5327-104">Při nasazení služby AD FS (Active Directory Federation Services) není pro síť intranet ve výchozím nastavení povoleno ověřování pomocí formulářů.</span><span class="sxs-lookup"><span data-stu-id="c5327-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="c5327-105">Pokud se integrované ověřování Windows nezdaří, zobrazí se výzva, abyste se přihlásili pomocí ověřování formulářů.</span><span class="sxs-lookup"><span data-stu-id="c5327-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="c5327-106">Tento problém vyřešíte tak, že povolíte ověřování pomocí formulářů v počítači s místní kopií služby Active Directory v konzole Microsoft Management Console (MMC) AD FS.</span><span class="sxs-lookup"><span data-stu-id="c5327-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="c5327-107">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="c5327-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="c5327-108">V navigačním podokně přejděte na **zásady ověřování**.</span><span class="sxs-lookup"><span data-stu-id="c5327-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="c5327-109">V části **Akce** v podokně Podrobnosti vyberte **Upravit globální primární ověřování**.</span><span class="sxs-lookup"><span data-stu-id="c5327-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="c5327-110">Na kartě **intranet** vyberte **ověřování formulářů**.</span><span class="sxs-lookup"><span data-stu-id="c5327-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="c5327-111">Vyberte **OK** (nebo **použít**).</span><span class="sxs-lookup"><span data-stu-id="c5327-111">Select **OK** (or **Apply**).</span></span>