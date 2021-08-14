---
title: SharePoint Problémy s připojením návrháře
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942018"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problémy s připojením návrháře 

Pokud SharePoint Designeru dochází k problémům s připojením SharePoint webů, vyzkoušejte následující společná řešení.

Krok 1: Ověřte, že je SharePoint Designer 2013 aktualizován pomocí [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a aktualizace z [2. srpna 2016 pro SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Vymazání souborů místní mezipaměti:

1. Zavřete SharePoint Designer 2013.

2. V místním počítači odeberte všechny soubory nalezené v každé z následujících složek.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otevřete SharePoint Designer 2013 a zadejte účet znovu, abyste viděli, jestli to funguje.

Krok 3: Povolte moderní ověřování [pro Office 2013 na Windows zařízeních.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Krok 4: Správci  budou muset povolit vlastní skript v nastavení SharePoint Admin Center, aby připojení SharePoint Designeru. Další [informace najdete v tématu Povolení nebo](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) zabránění vlastního skriptu.


