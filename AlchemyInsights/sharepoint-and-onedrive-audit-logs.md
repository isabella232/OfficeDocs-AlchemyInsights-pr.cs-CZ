---
title: Klasické sestavy protokolu auditování služby SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662201"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="72ef2-102">Protokoly auditování SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="72ef2-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="72ef2-103">Protokoly auditování klasické verze SharePointu</span><span class="sxs-lookup"><span data-stu-id="72ef2-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="72ef2-104">SPO starší auditování bylo migrováno do protokolu Unified audit (UAL).</span><span class="sxs-lookup"><span data-stu-id="72ef2-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="72ef2-105">Všechny SPO sestavy auditování starší verze teď budou napájeny přes UAL a starší signály auditu byly migrovány do UAL.</span><span class="sxs-lookup"><span data-stu-id="72ef2-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="72ef2-106">Klíčové změny:</span><span class="sxs-lookup"><span data-stu-id="72ef2-106">Key changes:</span></span>

* <span data-ttu-id="72ef2-107">Střih není k dispozici jako možnost.</span><span class="sxs-lookup"><span data-stu-id="72ef2-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="72ef2-108">Výběr konkrétních událostí k auditování není k dispozici.</span><span class="sxs-lookup"><span data-stu-id="72ef2-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="72ef2-109">V [tomto dokumentu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) najdete úplný seznam auditovaných událostí, které jsou ve výchozím nastavení dostupné.</span><span class="sxs-lookup"><span data-stu-id="72ef2-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="72ef2-110">Možnost **umístění** v části **přizpůsobené sestavy** není dostupná.</span><span class="sxs-lookup"><span data-stu-id="72ef2-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="72ef2-111">Možnost **otevřít nebo stáhnout dokumenty** není dostupná.</span><span class="sxs-lookup"><span data-stu-id="72ef2-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="72ef2-112">Konfigurace nastavení auditování pro kolekci webů</span><span class="sxs-lookup"><span data-stu-id="72ef2-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="72ef2-113">Moderní protokoly pro jednotné auditování v SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="72ef2-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="72ef2-114">Zapnutí nebo vypnutí protokolování jednotného auditu</span><span class="sxs-lookup"><span data-stu-id="72ef2-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="72ef2-115">V SharePointu nebo OneDrivu se nevyžaduje žádná další konfigurace.</span><span class="sxs-lookup"><span data-stu-id="72ef2-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="72ef2-116">Použití vyhledávání protokolování auditu ke kontrole aktivit souborů, složek, uživatelů, oprávnění:</span><span class="sxs-lookup"><span data-stu-id="72ef2-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="72ef2-117">Aktivity se soubory a stránkami</span><span class="sxs-lookup"><span data-stu-id="72ef2-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="72ef2-118">Aktivity složky</span><span class="sxs-lookup"><span data-stu-id="72ef2-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="72ef2-119">Aktivity sdílení a žádostí o přístup</span><span class="sxs-lookup"><span data-stu-id="72ef2-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="72ef2-120">Aktivity synchronizace</span><span class="sxs-lookup"><span data-stu-id="72ef2-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="72ef2-121">Aktivity správy webu</span><span class="sxs-lookup"><span data-stu-id="72ef2-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="72ef2-122">Další informace o tom, jak tyto události získat, najdete v tématu [vyhledání protokolu auditování](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="72ef2-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
