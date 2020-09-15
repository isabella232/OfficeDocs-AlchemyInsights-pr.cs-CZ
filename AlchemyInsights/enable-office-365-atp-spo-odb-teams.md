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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="0f6b4-102">365 povolení rozšířené ochrany před internetovými útoky pro SharePoint Online, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0f6b4-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="0f6b4-103">Přejděte na https://protection.office.com .</span><span class="sxs-lookup"><span data-stu-id="0f6b4-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="0f6b4-104">Zvolte **Threat management**  >  **Policy**  >  **zabezpečené přílohy**zásad správy hrozeb.</span><span class="sxs-lookup"><span data-stu-id="0f6b4-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="0f6b4-105">Vyberte **zapnout ATP pro SharePoint, OneDrive a Microsoft Teams**a pak klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="0f6b4-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="0f6b4-106">Doporuč Jako globální správce nebo správce SharePointu Online spusťte rutinu [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.</span><span class="sxs-lookup"><span data-stu-id="0f6b4-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="0f6b4-107">Doporuč [Nastavení upozornění](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pro zjištěné soubory</span><span class="sxs-lookup"><span data-stu-id="0f6b4-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="0f6b4-108">ATP bude rozvěřit všechny jednotlivé soubory v SharePointu Online, OneDrivu nebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0f6b4-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="0f6b4-109">Soubory jsou prohledávány asynchronně pomocí procesu, který využívá události sdílení a host, spolu s inteligentními heuristickými a signály pro hrozby k identifikaci nebezpečných souborů.</span><span class="sxs-lookup"><span data-stu-id="0f6b4-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="0f6b4-110">Podívejte [se na ATP pro SharePoint, OneDrive a Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="0f6b4-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>