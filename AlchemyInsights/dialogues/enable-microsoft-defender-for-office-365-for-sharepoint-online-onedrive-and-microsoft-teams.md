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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="94fd2-102">Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="94fd2-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="94fd2-103">Přihlaste se do Centra zabezpečení a dodržování předpisů [Office 365](https://protection.office.com/)pomocí přihlašovacích údajů globálního správce nebo správce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="94fd2-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="94fd2-104">V **levém podokně vyberte** Správu hrozeb a potom vyberte Přílohy **zásad**  >  [pro zabezpečení.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="94fd2-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="94fd2-105">Vyberte **Zapnout Microsoft Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams a pak vyberte **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="94fd2-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="94fd2-106">Jako globální správce nebo správce SharePointu Online spusťte tuto rutinu PowerShellu s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="94fd2-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="94fd2-107">Nastavení upozornění na zjištěné soubory</span><span class="sxs-lookup"><span data-stu-id="94fd2-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="94fd2-108">Další informace najdete v tématu [Microsoft Defender pro Office 365 pro SharePoint, OneDrive](https://go.microsoft.com/fwlink/?linkid=2092041)a Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="94fd2-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
