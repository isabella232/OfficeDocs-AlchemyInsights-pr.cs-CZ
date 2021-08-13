---
title: Omezení popisků citlivosti pro Office souborů v SharePoint a OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813151"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Omezení popisků citlivosti pro Office souborů v SharePoint a OneDrive

Při povolování popisků citlivosti pro Office souborů v SharePoint a OneDrive si uvědomte požadavky a omezení, mezi které patří:

- SharePoint OneDrive nemůže zpracovat některé soubory označené Office zašifrované z desktopových aplikací, když soubory obsahují data PowerQuery, data uložená vlastními doplňky nebo vlastní části XML.
- SharePoint a OneDrive na existující soubory, které jste už zašifrované pomocí štítků Azure Information Protection (AIP) automaticky nepou3/4ít popisky citlivosti. Použití popisků citlivosti u zašifrovaných souborů: 
    - Ujistěte se, že popisky AIP byly migrovány a publikovány do centra Microsoft 365 dodržování předpisů.
    - Stáhněte si označené soubory a pak je nahrajte do původního SharePoint nebo OneDrive umístění.
- U zašifrovaných dokumentů není tisk podporovaný.

Další podrobnosti o omezeních najdete v tématu Povolení popisků citlivosti [Office souborů v SharePoint](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)a OneDrive .
