---
title: Microsoft Defender pro Office 365 pro SharePoint, OneDrive a Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543570"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a7e9c-102">Microsoft Defender pro Office 365 pro SharePoint, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a7e9c-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a7e9c-103">Pokud chcete povolit Microsoft Defender pro Office 365:</span><span class="sxs-lookup"><span data-stu-id="a7e9c-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="a7e9c-104">Přejděte na účet globálního správce nebo správce [https://protection.office.com](https://protection.office.com) zabezpečení a přihlaste se.</span><span class="sxs-lookup"><span data-stu-id="a7e9c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a7e9c-105">V levém navigačním podokně v části **Správa hrozeb** zvolte **Bezpečné** \> **přílohy zásad**.</span><span class="sxs-lookup"><span data-stu-id="a7e9c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a7e9c-106">Vyberte **Zapnout Defender pro Office 365 pro SharePoint, OneDrive** a Microsoft Teams .</span><span class="sxs-lookup"><span data-stu-id="a7e9c-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a7e9c-107">[Vytvořte zásadu upozornění na aktivitu,](/microsoft-365/compliance/create-activity-alerts) která vám bude při zjišťování škodlivých souborů dostávat oznámení.</span><span class="sxs-lookup"><span data-stu-id="a7e9c-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a7e9c-108">Úplné pokyny najdete v tomto článku Zapnutí bezpečných příloh pro [SharePoint, OneDrive](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)a Microsoft Teams .</span><span class="sxs-lookup"><span data-stu-id="a7e9c-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a7e9c-109">**Poznámka:** Microsoft Defender pro Office 365 neskenuje každý jednotlivý soubor v SharePoint Online, OneDrive pro firmy nebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a7e9c-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a7e9c-110">Soubory se asynchronně naskenují procesem, který k identifikaci škodlivých souborů používá aktivity sdílení, aktivity hosta a signály hrozeb.</span><span class="sxs-lookup"><span data-stu-id="a7e9c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a7e9c-111">Další informace najdete v tématu [Bezpečné přílohy pro SharePoint, OneDrive](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)a Microsoft Teams .</span><span class="sxs-lookup"><span data-stu-id="a7e9c-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
