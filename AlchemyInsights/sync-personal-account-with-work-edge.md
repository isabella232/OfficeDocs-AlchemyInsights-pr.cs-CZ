---
title: Povolení uživateli synchronizovat osobní účet s pracovním účtem v Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813391"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Povolení uživateli synchronizovat osobní účet s pracovním účtem v Microsoft Edge

Ujistěte se, že splňujete tato kritéria:

- Enterprise Stavový roaming je povolený v Centru Azure Active Directory správy, které vyžaduje předplatné pro Azure Active Directory Premium nebo Enterprise Mobility + Security (EMS). Další informace najdete v článku [Povolení Enterprise roamingu v Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Jedno nebo obě z těchto kritérií jsou splněné:
    - Služba Azure Information Protection je pro vašeho tenanta povolená. Podrobnosti najdete v tématu [Aktivace ochrany Azure Rights Management z Centrum pro správu Microsoftu 365](/azure/information-protection/activate-office365).
    - Funkce Azure Active Directory Enterprise (ESR) je povolená pro libovolného uživatele nebo tenanta. Další informace najdete v tématu [Co je roaming v podnikovém stavu?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Pokud jsou funkce AIP i ESR zakázané, zobrazí se chybová zpráva oznamuje uživatelům, že synchronizace není pro jejich účty dostupná.
