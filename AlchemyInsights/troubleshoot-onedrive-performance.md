---
title: Odstraňování potíží s výkonem OneDrivu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757878"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="6859a-102">Odstraňování potíží s výkonem OneDrivu</span><span class="sxs-lookup"><span data-stu-id="6859a-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="6859a-103">Pokud máte pomalejší než očekávaná synchronizace nebo podobné problémy s výkonem s OneDrivem:</span><span class="sxs-lookup"><span data-stu-id="6859a-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="6859a-104">Ověřte, že neexistují žádné známé problémy s použitím [řídicího panelu stavu služby](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="6859a-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="6859a-105">[Povolte soubory na vyžádání](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , abyste měli přístup ke všem souborům na OneDrivu, aniž byste je museli stahovat a používat místo v zařízení.</span><span class="sxs-lookup"><span data-stu-id="6859a-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="6859a-106">[Přečtěte si Doporučené postupy](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) pro plánování sítě a výkon.</span><span class="sxs-lookup"><span data-stu-id="6859a-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="6859a-107">[Maximální rychlost nahrávání a stahování](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), zejména pokud právě synchronizujete zařízení.</span><span class="sxs-lookup"><span data-stu-id="6859a-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="6859a-108">Pokud synchronizujete knihovnu s víc než 100 000 položkami, může synchronizace OneDrivu zdánlivě trvat dlouhou dobu, nebo stav zobrazuje zpracování 0KB xMB. "</span><span class="sxs-lookup"><span data-stu-id="6859a-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="6859a-109">[Přečtěte si další informace o synchronizaci více než 100 000 souborů](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) a [maximálního podporovaného limitu souborů 300 000 na OneDrivu](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="6859a-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="6859a-110">Když uživatel překročí limit využití, SharePoint Online omezí všechny další žádosti tohoto uživatelského účtu na krátkou dobu.</span><span class="sxs-lookup"><span data-stu-id="6859a-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="6859a-111">Všechny akce uživatele jsou omezeny, pokud je v platnosti.</span><span class="sxs-lookup"><span data-stu-id="6859a-111">All user actions are throttled while the throttle is in effect.</span></span>
