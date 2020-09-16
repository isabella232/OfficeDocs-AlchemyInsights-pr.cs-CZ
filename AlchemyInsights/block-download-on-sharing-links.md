---
title: Blokování stahování v odkazech ke sdílení
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685735"
---
# <a name="block-download-on-sharing-links"></a>Blokování stahování v odkazech ke sdílení

**Blokové stahování** je k dispozici **jen pro odkazy** na dokumenty Office. Když vyberete tuto možnost, lidé, kteří získají přístup k souboru prostřednictvím vytvořeného odkazu, nebudou vidět možnosti pro stažení, tisk nebo kopírování souboru.

Správci můžou určit, jestli se má nastavení blokovat stahování zobrazovat jenom pro soubory Office, nebo změnit `BlockDownloadLinksFileType` nastavení v rutinách [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) nebo [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShellu.
