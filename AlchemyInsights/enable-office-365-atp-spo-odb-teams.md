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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543921"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams

1. Přejděte na https://protection.office.com stránku a přihlaste se.
2. Zvolte **Zásady správy**  >  **hrozeb**  >  **– bezpečné přílohy**.
3. Vyberte **Zapnout Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams a potom klikněte na **Uložit.**
4. (Doporučeno) Jako globální správce nebo správce SharePoint Online spusťte rutinu [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.
5. (Doporučeno) [Nastavení upozornění pro](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) zjištěné soubory

> [!NOTE]
> Microsoft Defender pro Office 365 neskenuje každý soubor v SharePoint Online, OneDrive nebo Microsoft Teams. Soubory se naskenují asynchronně prostřednictvím procesu, který používá události sdílení a hostování, spolu s inteligentní heuristikami a signály hrozeb k identifikaci škodlivých souborů. Informace [o Office 365, SharePoint, OneDrive](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a Microsoft Teams najdete v tématu Microsoft Defender.