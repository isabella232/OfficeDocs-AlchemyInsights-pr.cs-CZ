---
title: Služba Active Directory se nesynchronizuje
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697622"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="48906-102">Služba Active Directory se nesynchronizuje</span><span class="sxs-lookup"><span data-stu-id="48906-102">Active Directory not syncing</span></span>

<span data-ttu-id="48906-103">Pokud se vám zobrazují chyby synchronizace, třeba "žádná nedávná synchronizace" nebo se zobrazí stav synchronizace adresářů na portálu pro správu Office, znamená to, že se "naposledy synchronizace před více než 3 dny" znamená, že AADConnect má nesprávné nastavení nebo nemáte dostatečná oprávnění k provedení synchronizace.</span><span class="sxs-lookup"><span data-stu-id="48906-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="48906-104">Přeinstalace AADConnect pomocí expresního nastavení se dá použít k rychlému vyřešení problému:</span><span class="sxs-lookup"><span data-stu-id="48906-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="48906-105">[Stáhněte si nejnovější verzi AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="48906-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="48906-106">[Postupujte podle pokynů pro expresní instalaci](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="48906-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="48906-107">Další informace o účtech služeb AADConnect najdete v článku [Azure AD Connect: účty a oprávnění](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="48906-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
