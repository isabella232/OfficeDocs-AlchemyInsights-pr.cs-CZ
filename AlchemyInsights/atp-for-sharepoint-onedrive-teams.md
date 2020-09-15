---
title: ATP pro SharePoint, OneDrive a Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715554"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP pro SharePoint, OneDrive a Microsoft Teams

Pokud chcete zapnout rozšířenou ochranu před internetovými útoky, postupujte takto:

1. Přejděte na stránku [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí globálního správce nebo účtu správce zabezpečení.

2. V levém navigačním podokně v části **Správa hrozeb**zvolte **Policy** \> **zabezpečené přílohy**zásad.

3. Vyberte **zapnout ATP pro SharePoint, OneDrive a Microsoft Teams**.

4. [Vytvořte zásady upozornění na aktivitu](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , abyste mohli dostávat oznámení o škodlivých souborech.

Podrobné pokyny najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Poznámka**: v tomto designu nekontroluje ATP všechny jednotlivé soubory v SharePointu Online, OneDrivu pro firmy nebo Microsoft Teams. Soubory jsou prohledávány asynchronně procesem, který používá sdílení aktivity, aktivity hosta a signály hrozeb k identifikaci nebezpečných souborů. Další informace najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
