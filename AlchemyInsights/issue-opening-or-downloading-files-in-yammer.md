---
title: Problém s otevíráním nebo stahováním souborů v Yammer
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
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028243"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problém s otevíráním nebo stahováním souborů v Yammer

Klasické Yammer podporuje více možností pro nahrávání souborů do zpráv a skupin. V závislosti na konfiguraci sítě jsou soubory ve výchozím nastavení úložiště SharePoint.

Výběr souboru v novém Yammer zatím nepodporuje všechny možnosti dostupné v klasickém Yammer. Budoucí aktualizace přidá další funkce. Další informace najdete v tématu Připojení souboru nebo obrázku k příspěvku [Yammer konverzace.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**Soubor se nedaří otevřít nebo stáhnout.**  

Soubor se může nahrát do Yammer ale taky odkazovat na soubor v SharePoint Online. Pokud chcete vyřešit potíže, musíte nejdřív určit umístění souboru. Pokud byl soubor nahraný Yammer, bude mít adresu URL *.yammer.com. Ujistěte se, že jsou požadované adresy URL a IP adresy odblokované. Další informace najdete v blogu Použití pevných IP adres pro Yammer [nedoporučujeme.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Zkontrolujte, jestli si může soubor stáhnout i uživatel, který je také globálním správcem. Pokud je soubor soukromý, budete možná muset použít režim privátního obsahu. Další informace najdete v článku Sledování [soukromého obsahu v Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer a soubory na úrovni sítě v SharePoint Online**  

[Hosté na úrovni](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) sítě v Yammer nepoužívejte Azure AD B2B a jsou interní pro službu Yammer, takže nemají přístup k Yammer souborům uloženým v SharePoint. Vytvořte externího uživatele AAD B2B, který má přístup ke knihovnám dokumentů v SharePoint Online pomocí této identity. Informace o budoucí podpoře hosta Azure AD B2B v Yammer najdete v tématu Podpora hostů mezi firmami [(B2B)](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)v tématu Yammer Preview – Podmínky zákazníka a časté otázky .