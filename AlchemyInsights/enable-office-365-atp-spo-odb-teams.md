---
title: Povolení ATP Office 365 pro SharePoint, OneDrive a Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709900"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>365 povolení rozšířené ochrany před internetovými útoky pro SharePoint Online, OneDrive a Microsoft Teams

1. Přejděte na https://protection.office.com .
2. Zvolte **Threat management**  >  **Policy**  >  **zabezpečené přílohy**zásad správy hrozeb.
3. Vyberte **zapnout ATP pro SharePoint, OneDrive a Microsoft Teams**a pak klikněte na **Uložit**.
4. Doporuč Jako globální správce nebo správce SharePointu Online spusťte rutinu [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.
5. Doporuč [Nastavení upozornění](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pro zjištěné soubory

> [!NOTE]
> ATP bude rozvěřit všechny jednotlivé soubory v SharePointu Online, OneDrivu nebo Microsoft Teams. Soubory jsou prohledávány asynchronně pomocí procesu, který využívá události sdílení a host, spolu s inteligentními heuristickými a signály pro hrozby k identifikaci nebezpečných souborů. Podívejte [se na ATP pro SharePoint, OneDrive a Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).