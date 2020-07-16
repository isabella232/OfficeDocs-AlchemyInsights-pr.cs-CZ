---
title: Problém s otevíráním nebo stahováním souborů v Yammeru
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148204"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problém s otevíráním nebo stahováním souborů v Yammeru

Klasický Yammer podporuje více možností pro nahrávání souborů do zpráv a skupin. V závislosti na konfiguraci sítě jsou soubory výchozí pro úložiště v SharePointu.

Výběr souborů v novém Yammeru ještě nepodporuje všechny možnosti dostupné v klasickém Yammeru. Budoucí aktualizace přidá další funkce. Další informace najdete v [tématu Připojení souboru nebo obrázku k příspěvku konverzace na Yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Soubor nelze otevřít ani stáhnout.**  

Soubor se může nahrát do Yammeru, ale taky se propojí se souborem v SharePointu Online. Chcete-li odstranit potíže, musíte nejprve určit umístění souboru. Pokud byl soubor odeslán do Yammeru, bude mít adresu URL *.yammer.com. Ujistěte se, že jsou odblokovány požadované adresy URL a IP adresy. Další informace najdete v příspěvku blogu [Použití pevně kódovaných IP adres pro Yammer se nedoporučuje](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Zkontrolujte, zda uživatel, který je také globálním správcem, může soubor stáhnout. Pokud je soubor soukromý, bude pravděpodobně muset použít režim soukromého obsahu. Další informace najdete v [tématu Sledování soukromého obsahu v Yammeru](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Hosté a soubory na úrovni Yammeru na úrovni sítě v SharePointu Online**  

[Hosté na úrovni sítě v Yammeru](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nepoužívají Azure AD B2B a jsou interní pro službu Yammer, takže nemají přístup k souborům Yammeru uloženým v SharePointu. Vytvořte externího uživatele AAD B2B, který má přístup ke knihovnám dokumentů v SharePointu Online pomocí této identity. Informace o budoucí podpoře hosta Azure AD B2B v Yammeru najdete v tématu [Podpora hostů typu Business-to-business (B2B) ve verzi Yammer Preview – smluvní podmínky a nejčastější dotazy](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).