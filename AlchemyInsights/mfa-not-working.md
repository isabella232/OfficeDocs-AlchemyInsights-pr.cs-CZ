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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098595"
---
# <a name="issues-with-azure-mfa"></a>Problémy s Azure MFA
Existuje několik věcí, které můžete zkontrolovat, jestli se uživatelé nemohou přihlásit pomocí vícefaktorového ověřování (MFA).

1. Ovlivněný uživatel může být v Azure Active Directory Portálu zablokovaný. V takovém případě se pokusy o ověření pro tohoto konkrétního uživatele automaticky zamítne. [Postupujte podle pokynů v tomto článku a odblokujte je.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Pokud odblokování uživatele nepomáhá nebo uživatel není zablokovaný, můžete zkusit resetovat MFA pro uživatele a znovu projde procesem registrace. [Postupujte podle pokynů v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Pokud je to poprvé, co jste povolili MFA a vaši uživatelé se nebudou moci přihlásit k klientům, které nejsou prohlížeči, jako jsou Outlook, Skype atd., možná U předplatného O365 není povolená knihovna ADAL (Active Directory Authentication Library). V takovém případě se budete muset připojit k powershellu Exchange Online spustit tuto rutinu: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*