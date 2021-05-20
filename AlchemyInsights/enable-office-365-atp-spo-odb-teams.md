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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9d4eb-102">Povolení programu Microsoft Defender pro Office 365 pro SharePoint Online, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9d4eb-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="9d4eb-103">Přejděte na https://protection.office.com stránku a přihlaste se.</span><span class="sxs-lookup"><span data-stu-id="9d4eb-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="9d4eb-104">Zvolte **Zásady správy**  >  **hrozeb**  >  **– bezpečné přílohy**.</span><span class="sxs-lookup"><span data-stu-id="9d4eb-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="9d4eb-105">Vyberte **Zapnout Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams a potom klikněte na **Uložit.**</span><span class="sxs-lookup"><span data-stu-id="9d4eb-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="9d4eb-106">(Doporučeno) Jako globální správce nebo správce SharePoint Online spusťte rutinu [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrem **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.</span><span class="sxs-lookup"><span data-stu-id="9d4eb-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="9d4eb-107">(Doporučeno) [Nastavení upozornění pro](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) zjištěné soubory</span><span class="sxs-lookup"><span data-stu-id="9d4eb-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="9d4eb-108">Microsoft Defender pro Office 365 neskenuje každý soubor v SharePoint Online, OneDrive nebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9d4eb-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="9d4eb-109">Soubory se naskenují asynchronně prostřednictvím procesu, který používá události sdílení a hostování, spolu s inteligentní heuristikami a signály hrozeb k identifikaci škodlivých souborů.</span><span class="sxs-lookup"><span data-stu-id="9d4eb-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="9d4eb-110">Informace [o Office 365, SharePoint, OneDrive](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a Microsoft Teams najdete v tématu Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="9d4eb-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>