---
title: Zpětný zápis hesla nefunguje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324916"
---
# <a name="password-writeback-is-not-working"></a>Zpětný zápis hesla nefunguje

**Mám problémy s konfigurací zpětného zápisu hesla**

- Zpětný zápis hesla je prémiová funkce.
- Ujistěte se, že rozumíte licenčním požadavkům:
  - Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.
  - **Jenom uživatelé cloudu** – všechny placené skladové Office 365 (O365) nebo Azure AD Basic
  - **Cloud a/nebo** místní uživatelé – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
    - Další informace o požadavcích na licencování najdete v tématu [Licenční požadavky pro samoobslužné resetování hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Máte aspoň jeden účet správce a jeden testovací uživatelský účet s jednou z příslušné licence.
- Aby funkce zpětného zápisu hesla fungovala, musíte Připojení azure AD k primárnímu řadiči domény Emulator heslo. Službu Azure AD Připojení primární řadič domény můžete nakonfigurovat tak,  že kliknete pravým tlačítkem myši na vlastnosti synchronizačního konektoru služby Active Directory a pak vyberete **Konfigurovat oddíly adresářů**. Odtud vyhledejte oddíl  nastavení připojení řadiče domény a zaškrtněte políčko s názvem používat jenom **upřednostňované řadiče domény**.
    **Poznámka:** Pokud upřednostňovaný řadič domény není emulátor primárního řadiče domény, azure AD Připojení se k primárnímu řadiči domény pro zpětný zápis hesla přesto dostanete.
- Resetování hesla bylo ve vašem tenantovi nakonfigurované a povolené. Další informace najdete v tématu [Povolení uživatelům resetovat hesla Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Ujistěte se, že účet správce, který se používá k povolení zpětného zápisu hesel, je účet správce cloudu (vytvořený v Azure AD, ne v místní službě AD).
- Máte jedno nebo více doménovou strukturu místního nasazení ad se systémem Windows Server 2008 R2, Windows Server 2012 nebo Windows Server 2012 R2 s nainstalovanými nejnovějšími aktualizacemi Service Pack.
- Máte nainstalovaný nástroj Azure AD Připojení a připravili jste prostředí AD pro synchronizaci s cloudem. Před testováním zpětného zápisu hesla se ujistěte, že jste nejdřív dokončili úplnou import a úplnou synchronizaci ze služby AD i Azure AD v Azure AD Připojení.
- Další informace najdete v článku o tom, jak provést úplnou synchronizaci a [úplný import v Azure AD Připojení](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mám problém s připojením zpětného zápisu hesla**

1. Stáhněte si a povolte nejnovější verzi [Azure AD Připojení](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfigurace brány firewall: Nástroj Azure AD Připojení (1.1.443 a vyšší) bude potřebovat **odchozí přístup HTTPS** k:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Povolení trvalého zachování nečinných připojení po dobu nejméně 2–3 minut

**Pořád mám problémy s zpětným zápisem hesla**

- Pokud máte pořád potíže, zkuste zakázat a znovu povolit službu zpětného zápisu hesel v nástroji Azure AD Připojení.
- Další informace najdete v článku o zakázání a [opětovném povolení zpětného zápisu hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
