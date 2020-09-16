---
title: Problémy s připojením k SharePoint designeru
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727164"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s připojením k SharePoint designeru 

Pokud v aplikaci SharePoint Designer dochází k problémům s připojením k webům SharePoint, vyzkoušejte následující běžná řešení.

Krok 1: Ověřte, jestli je SharePoint Designer 2013 aktualizovaný pomocí [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [aktualizace 2016 pro SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: vymazání souborů místní mezipaměti:

1. Zavřete SharePoint Designer 2013.

2. V místním počítači odeberte všechny soubory nalezené ve všech následujících složkách.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otevřete SharePoint Designer 2013 a znovu zadejte účet, abyste viděli, jestli funguje.

Krok 3: [Povolte moderní ověřování pro Office 2013 na zařízeních s Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Krok 4: Správci budou muset povolit připojení k SharePoint designeru pomocí **vlastního skriptu** v nastavení centra pro správu SharePointu. Další informace najdete v tématu [Povolení nebo zakázání vlastního skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


