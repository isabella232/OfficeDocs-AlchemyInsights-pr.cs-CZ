---
title: Vytvoření webu v SharePointu Online
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
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732209"
---
# <a name="create-sharepoint-sites-using-templates"></a>Vytvoření SharePointových webů pomocí šablon

Možnost Uložit web jako šablonu není pro moderní komunikaci ani týmové weby podporovaná. Další informace o používání šablon najdete v článku [uložení, stažení a nahrání sharepointového webu jako šablony](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tady jsou některé běžné problémy a řešení týkající se uložení webu nebo seznamu jako šablony v SharePointu Online. 

**Tlačítko Uložit šablonu webu/seznamu není k dispozici nebo chybí**

Aby bylo možné povolit funkce šablony, musí správci povolit vlastní skript. Podrobné pokyny najdete v tématu Příklady a úvahy 

- [Povolení nebo zakázání vlastního skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Příkaz Uložit web jako šablonu není podporován a může způsobit problémy na webech, které používají infrastrukturu publikování serveru SharePoint Server.

**Šablonu webu nelze vytvořit nebo nefunguje správně**

V šabloně možná chybí [funkce](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje se. Pokud tuto funkci nelze aktivovat v aktuální kolekci webů, nelze k vytvoření webu použít šablonu webu.

- Zkontrolujte, jestli některé seznamy nebo knihovny nepřekročí [mezní hodnotu limit zobrazení seznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000.

- Web pravděpodobně používá příliš mnoho zdrojů, a proto šablona webu překračuje limit 50 MB.


- Vyskytly se problémy se zobrazením dat ze seznamu, který používá vyhledávací sloupec. Další informace najdete v tématu [seznam vygenerovaný šablonou nezobrazuje data ze správného vyhledávacího seznamu v SharePointu Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Podrobnější informace o běžných problémech a řešeních najdete v pro [vytváření a používání šablon webů](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



