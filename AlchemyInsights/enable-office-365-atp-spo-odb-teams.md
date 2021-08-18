---
title: Povolení Office 365 atp pro SharePoint, OneDrive a Microsoft Teams
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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332152"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams

1. Přejděte na https://protection.office.com stránku a přihlaste se.
2. Zvolte **Zásady správy**  >  **hrozeb Sejf**  >  **přílohy**.
3. Vyberte **Zapnout Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams a potom klikněte na **Uložit.**
4. (Doporučeno) Jako globální správce nebo správce SharePoint Online spusťte rutinu [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.
5. (Doporučeno) [Nastavení upozornění pro](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) zjištěné soubory

**Poznámka:** Microsoft Defender pro Office 365 neskenuje každý soubor v SharePoint Online, OneDrive nebo Microsoft Teams. Soubory se naskenují asynchronně prostřednictvím procesu, který používá události sdílení a hostování, spolu s inteligentní heuristikami a signály hrozeb k identifikaci škodlivých souborů. Další [informace o Office 365, SharePoint, OneDrive](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a Microsoft Teams najdete v tématu Microsoft Defender.
