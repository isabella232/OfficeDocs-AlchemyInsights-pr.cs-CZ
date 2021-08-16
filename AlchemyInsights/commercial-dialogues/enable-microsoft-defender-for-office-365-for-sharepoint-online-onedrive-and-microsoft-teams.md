---
title: Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058859"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams

1. Pomocí přihlašovacích údajů globálního správce nebo správce zabezpečení se přihlaste do Centra Office 365 zabezpečení a [dodržování předpisů](https://protection.office.com/).
2. V **levém podokně vyberte** Správa hrozeb a pak vyberte **Zásady**  >  [Sejf přílohy](https://protection.office.com/safeattachment).
3. Vyberte **Zapnout Microsoft Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams a pak vyberte **Uložit**.
    > [!TIP]
    >
    > - Jako globální správce nebo správce SharePoint Online spusťte následující rutinu PowerShellu s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Nastavení upozornění pro zjištěné soubory](https://go.microsoft.com/fwlink/?linkid=2092110)

Další informace najdete v tématu [Microsoft Defender for Office 365 for SharePoint, OneDrive](https://go.microsoft.com/fwlink/?linkid=2092041)a Microsoft Teams .
