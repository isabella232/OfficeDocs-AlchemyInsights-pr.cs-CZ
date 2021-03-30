---
title: Nápověda k nastavení zobrazení nočního osvětlení
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404266"
---
# <a name="help-with-the-night-light-display-setting"></a>Nápověda k nastavení zobrazení nočního osvětlení

Další informace o nastavení zobrazení v noční době najdete v tématu Nastavení zobrazení pro [noční dobu ve Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Pokud jsou možnosti nočního osvětlení v Nastavení šedé, zkontrolujte ovladač zobrazení: 

1. Klikněte na vyhledávací pole na hlavním panelu a  zadejte **Správce zařízení** a ve výsledcích hledání vyberte Správce zařízení.
1. Rozbalte **položku Grafické adaptéry**. 

Funkce nočního osvětlení bohužel není dostupná, pokud vaše zařízení používá ovladač DisplayLink nebo ovladač Základní displej.

Funkce nočního osvětlení používá nedávnou grafickou technologii, takže možná budete muset aktualizovat ovladač obrazovky:  

- Aktualizace můžete zkontrolovat tak, že v části **Spustit** aktualizaci  >    >  **nastavení & Windows**  >  **Update**  >  **vyhledat aktualizace**.  

NEBO

- Pokud chcete ručně stáhnout a nainstalovat nejnovější ovladače zobrazení, navštivte web podpory výrobce hardwaru.

## <a name="reset-night-light-in-the-registry"></a>Resetování nočního osvětlení v registru

Pokud aktualizace ovladače displeje nefunguje, bude možná potřeba obnovit noční osvětlení v registru.  

**Upozornění:** Tento krok řešení potíží se doporučuje jenom pro pokročilé uživatele. Pokud registr změníte nesprávně, může dojít k vážným problémům. Pokud chcete přidat ochranu, zálohujte registr před jeho úpravami, abyste ho mohli obnovit, pokud dojde k problémům.

1. Do vyhledávacího pole zadejte **regedit** a ve výsledcích hledání vyberte **Editor** registru.

1. Přejděte na následující klíč registru: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Export a odstranění následujícího podklíče:$$windows.data.bluelightreduction.bluelightreductionstate

1. Export a odstranění následujícího podklíče:$$windows.data.bluelightreduction.settings

1. Restartujte Windows a ověřte, jestli jsou dostupné možnosti nočního osvětlení.


