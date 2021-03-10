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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693247"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams

1. Přihlaste se do Centra zabezpečení a dodržování předpisů [Office 365](https://protection.office.com/)pomocí přihlašovacích údajů globálního správce nebo správce zabezpečení.
2. V **levém podokně vyberte** Správu hrozeb a potom vyberte Přílohy **zásad**  >  [pro zabezpečení.](https://protection.office.com/safeattachment)
3. Vyberte **Zapnout Microsoft Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams a pak vyberte **Uložit.**
    > [!TIP]
    >
    > - Jako globální správce nebo správce SharePointu Online spusťte tuto rutinu PowerShellu s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Nastavení upozornění na zjištěné soubory](https://go.microsoft.com/fwlink/?linkid=2092110)

Další informace najdete v tématu [Microsoft Defender pro Office 365 pro SharePoint, OneDrive](https://go.microsoft.com/fwlink/?linkid=2092041)a Microsoft Teams.
