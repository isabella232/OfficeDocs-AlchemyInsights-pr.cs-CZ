---
title: Vytvoření webu v SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057959"
---
# <a name="create-sharepoint-sites-using-templates"></a>Vytváření SharePoint webů pomocí šablon

Moderní komunikační ani týmové weby nepodporují možnost uložení webu jako šablony. Další informace o používání šablon si přečtěte v článku [Ukládání, stahování a nahrávání sharepointových webů jako šablon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tady jsou některé běžné problémy nebo řešení týkající se ukládání webu nebo seznamu jako šablony v Sharepointu Online. 

**Tlačítko Uložit šablonu webu nebo seznamu není k dispozici nebo chybí**

Správci budou muset Povolit vlastní skript, aby mohli zapnout funkce šablon. Podrobné kroky, příklady a důležité informace najdete v tématu 

- [Povolit nebo zakázat vlastní skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Příkaz Uložit web jako šablonu není podporovaný a může způsobit potíže s weby, které používají infrastrukturu publikování SharePoint Serveru.

**Šablonu webu nelze vytvořit nebo nefunguje správně.**

Šablona může chybět [a](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) neaktivuje se. Pokud tato funkce není dostupná k aktivaci v aktuální kolekci webů, nemůžete k vytvoření webu použít šablonu webu.

- Zkontrolujte, jestli nějaké seznamy nebo [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) knihovny překračují mezní hodnotu limitu zobrazení seznamu 5 000 položek, protože to může blokovat vytváření šablony webu.

- Web může používat příliš mnoho zdrojů, a proto šablona webu překračuje limit 50 MB.


- Existují problémy se zobrazením dat ze seznamu, který používá vyhledávací sloupec. Další informace najdete v článku Seznam generovaný šablonou nezobrazuje data ze správného vyhledávacího seznamu v [SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Podrobnější informace o běžných problémech a řešeních najdete v tématu [Vytváření a používání šablon webů](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



