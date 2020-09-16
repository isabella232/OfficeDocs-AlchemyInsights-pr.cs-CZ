---
title: Uložení webu nebo seznamu jako šablony
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727524"
---
# <a name="save-site-or-list-as-a-template"></a>Uložení webu nebo seznamu jako šablony

Šablony webů služby SharePoint jsou předdefinované definice navržené pro konkrétní podnik. Další informace najdete v tématu [použití šablon k vytvoření různých typů sharepointových webů](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tady jsou některé běžné problémy a řešení týkající se uložení webu nebo seznamu jako šablony v SharePointu Online.

**Tlačítko Uložit šablonu webu nebo seznamu není k dispozici nebo chybí**. 

- Aby bylo možné povolit funkce šablony, musí správci povolit vlastní skript. Podrobné pokyny najdete v části [Povolení nebo zakázání vlastního skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Příkaz Uložit web jako šablonu není podporován a může způsobit problémy na webech, které používají infrastrukturu publikování serveru SharePoint Server.


**Šablonu webu nelze vytvořit nebo nefunguje správně**

- V šabloně možná chybí [funkce](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje se. Pokud tuto funkci nelze aktivovat v aktuální kolekci webů, nelze k vytvoření webu použít šablonu webu.


- Zkontrolujte, jestli některé seznamy nebo knihovny nepřekročí [mezní hodnotu limit zobrazení seznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000.


- Web pravděpodobně používá příliš mnoho zdrojů, a proto šablona webu překračuje limit 50 MB.


- Vyskytly se problémy se zobrazením dat ze seznamu, který používá vyhledávací sloupec. Další informace najdete v tématu [seznam vygenerovaný šablonou nezobrazuje data ze správného vyhledávacího seznamu v SharePointu Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Podrobnější informace o běžných problémech a řešeních najdete v informacích o [vytváření a používání šablon webů](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

