---
title: Povolení Sejf příloh pro SharePoint, OneDrive a Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894456"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolení Sejf příloh pro SharePoint, OneDrive a Microsoft Teams

1. Pomocí přihlašovacích údajů globálního správce nebo správce zabezpečení otevřete portál Microsoft 365 Defender na webu a potom přejděte na Zásady & pravidla Zásady hrozeb Sejf Přílohy v <https://security.microsoft.com>  \>  \>  části **Zásady.**

   Pokud chcete přejít přímo na **Sejf přílohy,** použijte <https://security.microsoft.com/safeattachmentv2> .

2. Na stránce **Sejf Přílohy** klikněte na **Globální nastavení**.
3. V informačním seznamu, který se zobrazí, vyberte Zapnout Microsoft Defender pro Office 365 pro **SharePoint, OneDrive** a Microsoft Teams a pak vyberte **Uložit**.

    > [!TIP]
    >
    > Následujícím postupem zvýšíte ochranu příloh Sejf pro SharePoint, OneDrive a Microsoft Teams:
    >
    > - Pokud chcete uživatelům zabránit ve stahování škodlivých souborů, použijte hodnotu parametru `$true` *DisallowInfectedFileDownload* v **[rutině Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** v SharePoint Online PowerShellu. Další informace najdete v [článku Použití SharePoint Online PowerShellu](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)k zabránění uživatelům ve stahování škodlivých souborů .
    > - [Vytvoření zásad upozornění pro zjištěné soubory](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Další informace najdete v tématu Sejf přílohy Office 365 pro [SharePoint, OneDrive](https://go.microsoft.com/fwlink/?linkid=2092041)a Microsoft Teams .
