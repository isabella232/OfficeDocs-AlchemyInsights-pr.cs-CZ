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
# <a name="issues-with-azure-mfa"></a>Problémy s Azure MFA
Existuje několik věcí, jak zkontrolovat, jestli se uživatelé nemohou přihlásit pomocí vícefaktorového ověřování (MFA)

1. Ohrožený uživatel je pravděpodobně zablokován na portálu služby Azure Active Directory. V takovém případě budou pokusy o ověření pro daného uživatele automaticky odepřeny. [Odblokujte je podle pokynů v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Pokud se odblokování uživatele nepomůže nebo uživatel nezablokoval, můžete zkusit pro uživatele resetovat MFA a znovu ho provede. [Postupujte podle pokynů v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Pokud se jedná o první povolený MFA a vaši uživatelé se nemůžou přihlásit k neprohlížečovým klientům, jako je Outlook, Skype atd., možná v rámci předplatného O365 není povolená možnost ADAL (Active Directory Authentication Library). V tomto případě se musíte připojit k PowerShellu online Exchange a spustit tuto rutinu:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*