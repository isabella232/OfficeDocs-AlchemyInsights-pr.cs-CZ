---
title: Centrum pro správu Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826372"
---
# <a name="teams-admin-center"></a>Centrum pro správu Teams

Přečtěte si informace o správě Teams pomocí [centra pro správu Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Pokud nemůžete získat přístup k centru pro správu Teams, zkontrolujte následující položky:

- Zkontrolujte, jestli jste povolili příslušné [IP adresy a adresy URL Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na hraničních zařízeních (bráně firewall atd.) nebo v pravidlech brány firewall na místním počítači.
- Zkontrolujte, jestli přihlašovací jméno, které používáte pro přístup k portálu pro správu Teams, odpovídá vašemu uživatelskému jménu uvedenému na [portálu pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Pokud se v centru pro správu Teams neobjevují uživatelé, zkontrolujte následující položky:

- Vytvořili jste v posledních 24 hodinách uživatele nebo přiřazovali licence? Než otevřete lístek podpory, počkejte alespoň 24 hodin.
- Ověřte, že jste přiřadili správné licence.
- Pokud máte místní službu Active Directory, ověřte, jestli je hodnota [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) nebo adresy SIP v poli ProxyAddresses v místní službě Active Directory jedinečná a formát odpovídá sip:**Uživatelské** jméno uživatele z Centra pro správu [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Pokud máte v úmyslu zachovat nasazení Serveru Skypu pro firmy a mít uživatele místně a online: Postupujte podle pokynů v části Nastavení hybridního nasazení přes Teams a **Online Skypu** pro firmy v Ovládacích panelech serveru Skypu pro firmy a přesunutí uživatelů online.
