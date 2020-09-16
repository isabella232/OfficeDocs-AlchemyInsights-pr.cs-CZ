---
title: Problémy s MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755124"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="b8096-102">Problémy s Azure MFA</span><span class="sxs-lookup"><span data-stu-id="b8096-102">Issues with Azure MFA</span></span>
<span data-ttu-id="b8096-103">Existuje několik věcí, jak zkontrolovat, jestli se uživatelé nemohou přihlásit pomocí vícefaktorového ověřování (MFA)</span><span class="sxs-lookup"><span data-stu-id="b8096-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b8096-104">Ohrožený uživatel je pravděpodobně zablokován na portálu služby Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8096-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b8096-105">V takovém případě budou pokusy o ověření pro daného uživatele automaticky odepřeny.</span><span class="sxs-lookup"><span data-stu-id="b8096-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b8096-106">Odblokujte je podle pokynů v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="b8096-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b8096-107">Pokud se odblokování uživatele nepomůže nebo uživatel nezablokoval, můžete zkusit pro uživatele resetovat MFA a znovu ho provede.</span><span class="sxs-lookup"><span data-stu-id="b8096-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b8096-108">Postupujte podle pokynů v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="b8096-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b8096-109">Pokud se jedná o první povolený MFA a vaši uživatelé se nemůžou přihlásit k neprohlížečovým klientům, jako je Outlook, Skype atd., možná v rámci předplatného O365 není povolená možnost ADAL (Active Directory Authentication Library).</span><span class="sxs-lookup"><span data-stu-id="b8096-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b8096-110">V tomto případě se musíte připojit k PowerShellu online Exchange a spustit tuto rutinu:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="b8096-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>