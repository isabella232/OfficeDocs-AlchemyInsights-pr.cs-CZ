---
title: Active Directory se nesynchronuje
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822844"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="c18e0-102">Active Directory se nesynchronuje</span><span class="sxs-lookup"><span data-stu-id="c18e0-102">Active Directory not syncing</span></span>

<span data-ttu-id="c18e0-103">Pokud se vám zobrazí chyby synchronizace, například "žádná nedávná synchronizace", nebo si všimnete, že stav synchronizace adresářů na portálu pro správu Office říká: "Poslední synchronizace před více než 3 dny", může to být tím, že AADConnect má nesprávná nastavení nebo nedostatečná oprávnění k provedení synchronizace.</span><span class="sxs-lookup"><span data-stu-id="c18e0-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="c18e0-104">Přeinstalace AADConnect pomocí expresního nastavení může tento problém rychle vyřešit:</span><span class="sxs-lookup"><span data-stu-id="c18e0-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="c18e0-105">[Stáhněte si nejnovější verzi AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="c18e0-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="c18e0-106">[Postupujte podle pokynů pro expresní instalaci](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="c18e0-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="c18e0-107">Další informace o účtech služeb AADConnect najdete v tématu [Azure AD Connect: Účty](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)a oprávnění .</span><span class="sxs-lookup"><span data-stu-id="c18e0-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
