---
title: Problémy s MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810477"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="03af4-102">Problémy s Azure MFA</span><span class="sxs-lookup"><span data-stu-id="03af4-102">Issues with Azure MFA</span></span>
<span data-ttu-id="03af4-103">Existuje několik věcí, které můžete zkontrolovat, jestli se uživatelé nemohou přihlásit pomocí vícefaktorového ověřování (MFA).</span><span class="sxs-lookup"><span data-stu-id="03af4-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="03af4-104">Ovlivněný uživatel může být na portálu Azure Active Directory zablokovaný.</span><span class="sxs-lookup"><span data-stu-id="03af4-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="03af4-105">V takovém případě se pokusy o ověření pro tohoto konkrétního uživatele automaticky zamítne.</span><span class="sxs-lookup"><span data-stu-id="03af4-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="03af4-106">Postupujte podle pokynů v tomto článku a odblokujte je.</span><span class="sxs-lookup"><span data-stu-id="03af4-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="03af4-107">Pokud odblokování uživatele nepomáhá nebo uživatel není zablokovaný, můžete zkusit resetovat MFA pro uživatele a znovu projde procesem registrace.</span><span class="sxs-lookup"><span data-stu-id="03af4-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="03af4-108">Postupujte podle pokynů v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="03af4-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="03af4-109">Pokud je to poprvé, co jste povolili MFA a vaši uživatelé se nebudou moci přihlásit k klientům, které nejsou prohlížeči, jako je Outlook, Skype atd., možná U předplatného O365 není povolená knihovna ADAL (Active Directory Authentication Library).</span><span class="sxs-lookup"><span data-stu-id="03af4-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="03af4-110">V takovém případě se budete muset připojit k Powershellu Exchange Online a spustit tuto rutinu:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="03af4-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>