---
title: Zpoždění při přijímání upozornění SharePointu a OneDrivu
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785658"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Zpoždění při přijímání upozornění SharePointu a OneDrivu

- Nejdřív v e-mailu zkontrolujte nevyžádaná nebo Nevyžádaná pošta.
- Pokud **jsou všechny výstrahy z více souborů nebo knihoven zpožděné**, navštivte [řídicí panel stavu služeb](https://portal.office.com/adminportal/home?ref=/servicehealth) a zkontrolujte, jestli nejsou k dispozici žádné informační zpravodaje nebo události, které se můžou vyskytovat v SharePointu nebo Exchange. Problém může být v případě, že se jedná o možnost upozorňování SharePointu nebo zpoždění e-mailů prostřednictvím Exchange. Také si všimněte, jestli se dodávají další e-maily – Pokud ne, problém se může projevit zpoždění Exchange.
- Pokud není **doručeno konkrétní upozornění z určitého souboru nebo knihovny**, zkuste ho odstranit a znovu vytvořit. Další informace najdete v tématu [Správa, zobrazení nebo odstranění upozornění SharePointu](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Do distribuční skupiny nelze posílat upozornění. Podporují se jenom skupiny Security a O365.
> - E-mailové šablony nemůžete přizpůsobit. K dosažení těchto cílů musíte použít pracovní postup Microsoft Flow nebo SharePoint Designer.
