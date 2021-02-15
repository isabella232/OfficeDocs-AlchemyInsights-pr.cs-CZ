---
title: Nefunguje zpětný zápis hesla
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243287"
---
# <a name="password-writeback-is-not-working"></a>Nefunguje zpětný zápis hesla

**Mám problémy s konfigurací zpětného zápisu hesla**

- Zpětný zápis hesla je prémiová funkce.
- Ujistěte se, že rozumíte licenčním požadavkům:
  - Ve vaší organizaci musíte mít přiřazenou aspoň jednu licenci.
  - **Jenom cloudové uživatele** – všechny placené SKU Office 365 (O365) nebo Azure AD Basic
  - **Cloudové a místní** uživatele – Azure AD Premium P1 nebo P2, Enterprise Mobility + Security (EMS) nebo Secure Productive Enterprise (SPE)
    - Další informace o licenčních požadavcích najdete v článku o licenčních požadavcích pro samoobslužné [resetování hesla Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Máte aspoň jeden účet správce a jeden zkušební uživatelský účet s jednou z příslušné licence.
- Aby zpětné zapisování hesla fungovalo, musíte Připojit Azure AD Connect k emulátoru primárního řadiče domény. Azure AD Connect můžete nakonfigurovat tak, aby bylo  možné používat primární řadič domény, a to tak, že kliknete pravým tlačítkem na vlastnosti konektoru synchronizace služby Active Directory a pak vyberete **konfigurovat oddíly adresáře.** Odtud vyhledejte část  nastavení připojení řadičů domén a zaškrtněte políčko s názvem Používají se **jenom preferované řadiče domény.**
  > [!NOTE]
  > Pokud upřednostňovaný kód DC není emulátoru PDC, Azure AD Connect stále kontaktovat PDC kvůli zpětnému zápisu hesla.
- Resetování hesla je nakonfigurované a povolené ve vašem tenantovi. Další informace najdete v článku o tom, [jak uživatelům povolit resetování hesel Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Ujistěte se, že se účet správce, který se používá k povolení zpětného zápisu hesel, je účet cloudového správce (který se vytvořil v Azure AD ne v místní službě AD).
- Máte místní nasazení AD s jednou nebo více doménovou doménovou doménou, na které běží Windows Server 2008 R2, Windows Server 2012 nebo Windows Server 2012 R2 s nainstalovanými nejnovějšími aktualizacemi Service Pack.
- Máte nainstalovaný nástroj Azure AD Connect a máte připravené prostředí AD pro synchronizaci s cloudem. Před testováním zpětného zápisu hesel zkontrolujte, že je v Azure AD Connect nejprve dokončena úplná importovaná a úplná synchronizace ze služby AD i z Azure AD.
- Další informace najdete v článku o úplné synchronizaci a [úplném importu v Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mám potíže s připojením k zpětném zápisu hesla**

1. Stažení a povolení nejnovější verze [služby Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfigurace brány firewall: Nástroj Azure AD Connect (1.1.443 a vyšší) bude potřebovat **odchozí přístup HTTPS** pro:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Povolit nečinná připojení, aby se zachovávaly minimálně 2–3 minuty

**Pořád mám problémy s zpětným zápisem hesla**

- Pokud s tím budou problémy i nadále, zkuste zakázat a znovu povolit službu zpětného zápisu hesel v nástroji Azure AD Connect.
- Další informace najdete v článku o zakázání a [opětovném povolení zpětného zápisu hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
