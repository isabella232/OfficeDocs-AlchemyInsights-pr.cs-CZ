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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930968"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="b6c08-102">Active Directory se nesynchronuje</span><span class="sxs-lookup"><span data-stu-id="b6c08-102">Active Directory not syncing</span></span>

<span data-ttu-id="b6c08-103">Pokud se na portálu pro správu Office zobrazí chyby synchronizace, například "žádná nedávná synchronizace", nebo si všimnete stavu synchronizace adresářů na portálu pro správu Office, že se naposledy synchronizovala před více než 3 dny, může to být tím, že AADConnect má nesprávná nastavení nebo nemá dostatečná oprávnění k provedení synchronizace.</span><span class="sxs-lookup"><span data-stu-id="b6c08-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="b6c08-104">Přeinstalace AADConnect pomocí expresního nastavení může problém rychle vyřešit:</span><span class="sxs-lookup"><span data-stu-id="b6c08-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="b6c08-105">[Stáhněte si nejnovější verzi AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="b6c08-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="b6c08-106">[Postupujte podle pokynů pro expresní instalaci](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="b6c08-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="b6c08-107">Služba Azure AD Connect musí být nainstalovaná na Windows Serveru 2012 nebo novějším.</span><span class="sxs-lookup"><span data-stu-id="b6c08-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="b6c08-108">Tento server musí být připojený k doméně a může to být řadič domény nebo členský server.</span><span class="sxs-lookup"><span data-stu-id="b6c08-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="b6c08-109">Úplný seznam požadavků na služby Azure AD Připojení a předběžných požadavků naleznete v tématu Předpoklady pro [Azure AD Připojení](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="b6c08-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="b6c08-110">Další informace o účtech služeb AADConnect najdete v tématu [Azure AD Připojení: Účty](/azure/active-directory/hybrid/reference-connect-accounts-permissions)a oprávnění .</span><span class="sxs-lookup"><span data-stu-id="b6c08-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
