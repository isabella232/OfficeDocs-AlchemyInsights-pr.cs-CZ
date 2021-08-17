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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109197"
---
# <a name="save-site-or-list-as-a-template"></a>Uložení webu nebo seznamu jako šablony

SharePoint šablony webů jsou předem sestavené definice navržené tak, aby byly specifické pro firmy. Další informace najdete v tématu [Použití šablon k vytvoření různých](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)typů SharePoint webů .

Tady jsou některé běžné problémy nebo řešení týkající se uložení webu nebo seznamu jako šablony v SharePoint Online.

**Tlačítko Uložit šablonu webu nebo seznamu není k dispozici nebo chybí**. 

- Správci budou muset Povolit vlastní skript, aby mohli zapnout funkce šablon. Podrobné kroky, příklady a důležité informace najdete v tématu [Povolení nebo zabránění vlastního skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Příkaz Uložit web jako šablonu není podporovaný a může způsobit potíže s weby, které používají infrastrukturu publikování SharePoint Serveru.


**Šablonu webu nelze vytvořit nebo nefunguje správně.**

- Šablona může chybět [a](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) neaktivuje se. Pokud tato funkce není dostupná k aktivaci v aktuální kolekci webů, nemůžete k vytvoření webu použít šablonu webu.


- Zkontrolujte, jestli nějaké seznamy nebo [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) knihovny překračují mezní hodnotu limitu zobrazení seznamu 5 000 položek, protože to může blokovat vytváření šablony webu.


- Web může používat příliš mnoho zdrojů, a proto šablona webu překračuje limit 50 megabajtů (MB).


- Existují problémy se zobrazením dat ze seznamu, který používá vyhledávací sloupec. Další informace najdete v článku Seznam generovaný šablonou nezobrazuje data ze správného vyhledávacího seznamu v [SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Podrobnější informace o běžných problémech a řešeních najdete v [tématu Vytváření a používání šablon webů.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

