---
title: Určení aktivity pravidla doručené pošty v protokolech auditování
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779044"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="d583b-102">Určení aktivity pravidla doručené pošty v protokolech auditování</span><span class="sxs-lookup"><span data-stu-id="d583b-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="d583b-103">Pokud chcete zobrazit události pravidla doručené pošty (vytváření, úpravy a odstraňování pravidel doručené pošty), můžete použít vyhledávání v protokolu auditování v centru & zabezpečení Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d583b-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="d583b-104">Přihlaste se do [centra zabezpečení Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="d583b-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="d583b-105">Přejděte na stránku **Search**pro  >  **vyhledávání protokolu auditování** .</span><span class="sxs-lookup"><span data-stu-id="d583b-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="d583b-106">V polích **Datum zahájení** a **Datum ukončení** vyberte rozsah dat.</span><span class="sxs-lookup"><span data-stu-id="d583b-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="d583b-107">V části **aktivity poštovní schránky Exchange**ověřte, že pole **aktivity** je nastavené na **New-InboxRule**.</span><span class="sxs-lookup"><span data-stu-id="d583b-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="d583b-108">Klikněte na **Hledat**.</span><span class="sxs-lookup"><span data-stu-id="d583b-108">Click **Search**.</span></span>

<span data-ttu-id="d583b-109">Ve výsledcích vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="d583b-109">In the results, select an audit record.</span></span> <span data-ttu-id="d583b-110">V rozevíracím seznamu podrobností klikněte na **Další informace**.</span><span class="sxs-lookup"><span data-stu-id="d583b-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d583b-111">Informace o nastavení pravidla doručené pošty se zobrazí v poli **parametry** .</span><span class="sxs-lookup"><span data-stu-id="d583b-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="d583b-112">Další informace najdete v tématu [určení, jestli uživatel vytvořil pravidlo doručené pošty](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .</span><span class="sxs-lookup"><span data-stu-id="d583b-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
