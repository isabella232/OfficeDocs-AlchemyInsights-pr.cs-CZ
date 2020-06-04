---
title: Zpoždění při přijímání upozornění na SharePointu a OneDrivu
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563503"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Zpoždění při přijímání upozornění na SharePointu a OneDrivu

- Nejprve zkontrolujte složku Nevyžádaná pošta nebo Nevyžádaná pošta v e-mailu.
- Pokud **jsou všechny výstrahy z více souborů nebo knihoven zpožděny**, navštivte [řídicí panel Stav služby](https://portal.office.com/adminportal/home?ref=/servicehealth) a zkontrolujte, zda se u SharePointu nebo Exchange nevyskytují všechny informační zpravodaje nebo incidenty, ke kterým může dojít. Problém může být s funkcí upozornění SharePoint nebo zpoždění v e-mailech prostřednictvím exchange. Všimněte si také, zda jsou doručovány další e-maily – pokud ne, problém je pravděpodobně se zpožděním exchange.
- Pokud **není doručena jednotlivá výstraha z určitého souboru nebo knihovny**, pokuste se ji odstranit a znovu vytvořit. Viz [Správa, zobrazení nebo odstranění sharepointových výstrah,](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) abyste výstrahu znovu vytvořili.

> [!NOTE]
> - Výstrahy nelze odeslat distribuční skupině. Podporovány jsou pouze skupiny Zabezpečení a O365.
> - Šablony e-mailů s výstrahami nelze přizpůsobit. K jejich dosažení je nutné použít Microsoft Flow nebo SharePoint Designer Workflow.
