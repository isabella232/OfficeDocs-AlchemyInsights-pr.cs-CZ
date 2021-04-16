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
# <a name="issues-with-azure-mfa"></a>Problémy s Azure MFA
Existuje několik věcí, které můžete zkontrolovat, jestli se uživatelé nemohou přihlásit pomocí vícefaktorového ověřování (MFA).

1. Ovlivněný uživatel může být na portálu Azure Active Directory zablokovaný. V takovém případě se pokusy o ověření pro tohoto konkrétního uživatele automaticky zamítne. [Postupujte podle pokynů v tomto článku a odblokujte je.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Pokud odblokování uživatele nepomáhá nebo uživatel není zablokovaný, můžete zkusit resetovat MFA pro uživatele a znovu projde procesem registrace. [Postupujte podle pokynů v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Pokud je to poprvé, co jste povolili MFA a vaši uživatelé se nebudou moci přihlásit k klientům, které nejsou prohlížeči, jako je Outlook, Skype atd., možná U předplatného O365 není povolená knihovna ADAL (Active Directory Authentication Library). V takovém případě se budete muset připojit k Powershellu Exchange Online a spustit tuto rutinu:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*