---
title: Chyba Aplikace Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786662"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="e89aa-102">Chyba 4c7 v Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e89aa-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="e89aa-103">K této chybě dochází, protože Microsoft Teams vyžaduje ověřování pomocí formulářů.</span><span class="sxs-lookup"><span data-stu-id="e89aa-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="e89aa-104">Při nasazení služby AD FS (Active Directory Federation Services) není ověřování pomocí formulářů pro intranet ve výchozím nastavení povolené.</span><span class="sxs-lookup"><span data-stu-id="e89aa-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="e89aa-105">Pokud se integrované ověřování ve Windows nepodaří, zobrazí se výzva k přihlášení pomocí ověřování pomocí formulářů.</span><span class="sxs-lookup"><span data-stu-id="e89aa-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="e89aa-106">Chcete-li tento problém vyřešit, povolte ověřování pomocí modulu snap-in KONZOLA MICROSOFT MANAGEMENT CONSOLE (MMC) služby AD FS v počítači, který má místní kopii služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e89aa-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="e89aa-107">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="e89aa-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="e89aa-108">V navigačním podokně přejděte na **Zásady ověřování**.</span><span class="sxs-lookup"><span data-stu-id="e89aa-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="e89aa-109">V **části Akce** v podokně podrobností vyberte Upravit globální primární **ověřování**.</span><span class="sxs-lookup"><span data-stu-id="e89aa-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="e89aa-110">Na kartě **Intranet** vyberte Ověřování **pomocí formulářů**.</span><span class="sxs-lookup"><span data-stu-id="e89aa-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="e89aa-111">Vyberte **OK** (nebo **Použít).**</span><span class="sxs-lookup"><span data-stu-id="e89aa-111">Select **OK** (or **Apply**).</span></span>