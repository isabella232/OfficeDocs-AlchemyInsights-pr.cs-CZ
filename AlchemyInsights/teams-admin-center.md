---
title: Centrum pro správu Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670357"
---
# <a name="teams-admin-center"></a>Centrum pro správu Teams

Přečtěte si informace o správě Teams pomocí [centra pro správu Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Pokud nemůžete získat přístup k centru pro správu Teams, zkontrolujte následující položky:

- Zkontrolujte, jestli jste povolili příslušné [IP adresy a adresy URL Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na hraničních zařízeních (bráně firewall atd.) nebo v pravidlech brány firewall na místním počítači.
- Zkontrolujte, jestli přihlašovací jméno, které používáte pro přístup k portálu pro správu Teams, odpovídá vašemu uživatelskému jménu uvedenému na [portálu pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Pokud se v centru pro správu Teams neobjevují uživatelé, zkontrolujte následující položky:

- Vytvořili jste v posledních 24 hodinách uživatele nebo přiřazovali licence? Než otevřete lístek podpory, počkejte alespoň 24 hodin.
- Ověřte, že jste přiřadili správné licence.
- Pokud máte místní službu Active Directory, ověřte, že [hodnota parametru msRTCSIP-PrimaryUserAddress nebo adresy SIP v poli proxyAddresses v místní službě Active Directory je jedinečná a formát odpovídá](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) protokolu SIP:**uživatelské jméno** uživatele z [centra pro správu Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Pokud máte v úmyslu zachovat nasazení serveru Skype pro firmy a máte místní i online uživatele, postupujte podle pokynů v **části nastavení hybridu s týmy a Skypu pro firmy** na ovládacím panelu serveru Skype pro firmy a přesunutí uživatelů do online režimu.
