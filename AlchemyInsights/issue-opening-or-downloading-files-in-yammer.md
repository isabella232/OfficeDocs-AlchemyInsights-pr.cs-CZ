---
title: Vystavení otevírání nebo stahování souborů v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695642"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Vystavení otevírání nebo stahování souborů v Yammeru

Klasická Yammer podporuje více možností odesílání souborů do zpráv a skupin. V závislosti na konfiguraci sítě se jedná o výchozí nastavení souborů úložiště v SharePointu.

Výběr souborů v nové Yammeru zatím nepodporuje všechny možnosti dostupné v klasické Yammeru. Budoucí aktualizace přidá další funkce. Další informace najdete v článku [připojení souboru nebo obrázku ke příspěvku v konverzaci Yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Soubor nelze otevřít ani stáhnout**  

Soubor se může nahrát do Yammeru, ale taky se odkazuje na soubor v SharePointu Online. Abyste mohli řešit potíže, musíte nejdřív určit umístění souboru. Pokud se soubor nahrál na Yammer, bude mít adresu URL *. yammer.com. Zajistěte, aby se odblokovaly požadované adresy URL a IP adresy. Další informace najdete v článku příspěvek na blog [s použitím pevných kódovaných IP adres pro Yammer se nedoporučuje](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Zkontrolujte, jestli soubor stáhne uživatel, který je taky globálním správcem. Pokud je soubor soukromý, bude možná potřeba použít režim soukromého obsahu. Další informace najdete [v tématu sledování soukromého obsahu v Yammeru](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Hosté a soubory uživatelů Yammeru na úrovni sítě v SharePointu Online**  

[Hosté na úrovni sítě v Yammeru](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nepoužívají Azure AD B2B a jsou vnitřní pro službu Yammer, takže nemají přístup k souborům Yammeru uloženým na SharePointu. Pomocí této identity můžete vytvořit externího uživatele AAD, který má přístup ke knihovnám dokumentů v SharePointu Online. Informace o budoucí podpoře hostů služby Azure AD B2B v Yammeru najdete v článku [Podpora hostů mezi podniky (B2B) v části s informacemi o zákaznících a nejčastější dotazy](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).