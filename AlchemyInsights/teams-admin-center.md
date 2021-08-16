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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049337"
---
# <a name="teams-admin-center"></a>Centrum pro správu Teams

Přečtěte si informace o správě Teams pomocí [centra pro správu Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Pokud nemůžete získat přístup k centru pro správu Teams, zkontrolujte následující položky:

- Zkontrolujte, jestli jste povolili příslušné [IP adresy a adresy URL Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na hraničních zařízeních (bráně firewall atd.) nebo v pravidlech brány firewall na místním počítači.
- Zkontrolujte, jestli přihlašovací jméno, které používáte pro přístup k portálu pro správu Teams, odpovídá vašemu uživatelskému jménu uvedenému na [portálu pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Pokud se v centru pro správu Teams neobjevují uživatelé, zkontrolujte následující položky:

- Vytvořili jste v posledních 24 hodinách uživatele nebo přiřazovali licence? Než otevřete lístek podpory, počkejte alespoň 24 hodin.
- Ověřte, že jste přiřadili správné licence.
- Pokud máte místní službu Active Directory, ověřte, že hodnota [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) nebo adresa SIP v poli ProxyAddresses v místní službě Active Directory je jedinečná a formát odpovídá sip:**Uživatelské** jméno uživatele z [Centrum pro správu Microsoftu 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Pokud máte v úmyslu zachovat nasazení Server Skypu pro firmy a mít uživatele místně a online: postupujte podle pokynů v části Nastavení hybridního nasazení s Teams a **Skype pro firmy Online v** Ovládacích panelech Server Skypu pro firmy a přesouhněte uživatele online.
