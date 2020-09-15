---
title: ATP pro SharePoint, OneDrive a Microsoft Teams
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715554"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="c8f2c-102">ATP pro SharePoint, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c8f2c-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="c8f2c-103">Pokud chcete zapnout rozšířenou ochranu před internetovými útoky, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="c8f2c-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="c8f2c-104">Přejděte na stránku [https://protection.office.com](https://protection.office.com) a přihlaste se pomocí globálního správce nebo účtu správce zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c8f2c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="c8f2c-105">V levém navigačním podokně v části **Správa hrozeb**zvolte **Policy** \> **zabezpečené přílohy**zásad.</span><span class="sxs-lookup"><span data-stu-id="c8f2c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="c8f2c-106">Vyberte **zapnout ATP pro SharePoint, OneDrive a Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="c8f2c-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="c8f2c-107">[Vytvořte zásady upozornění na aktivitu](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) , abyste mohli dostávat oznámení o škodlivých souborech.</span><span class="sxs-lookup"><span data-stu-id="c8f2c-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="c8f2c-108">Podrobné pokyny najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c8f2c-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="c8f2c-109">**Poznámka**: v tomto designu nekontroluje ATP všechny jednotlivé soubory v SharePointu Online, OneDrivu pro firmy nebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c8f2c-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="c8f2c-110">Soubory jsou prohledávány asynchronně procesem, který používá sdílení aktivity, aktivity hosta a signály hrozeb k identifikaci nebezpečných souborů.</span><span class="sxs-lookup"><span data-stu-id="c8f2c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="c8f2c-111">Další informace najdete v tomto [tématu](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c8f2c-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
