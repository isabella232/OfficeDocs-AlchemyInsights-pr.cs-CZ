---
title: Zpoždění při přijímání upozornění na SharePointu a OneDrivu
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563503"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="57609-102">Zpoždění při přijímání upozornění na SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="57609-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="57609-103">Nejprve zkontrolujte složku Nevyžádaná pošta nebo Nevyžádaná pošta v e-mailu.</span><span class="sxs-lookup"><span data-stu-id="57609-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="57609-104">Pokud **jsou všechny výstrahy z více souborů nebo knihoven zpožděny**, navštivte [řídicí panel Stav služby](https://portal.office.com/adminportal/home?ref=/servicehealth) a zkontrolujte, zda se u SharePointu nebo Exchange nevyskytují všechny informační zpravodaje nebo incidenty, ke kterým může dojít.</span><span class="sxs-lookup"><span data-stu-id="57609-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="57609-105">Problém může být s funkcí upozornění SharePoint nebo zpoždění v e-mailech prostřednictvím exchange.</span><span class="sxs-lookup"><span data-stu-id="57609-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="57609-106">Všimněte si také, zda jsou doručovány další e-maily – pokud ne, problém je pravděpodobně se zpožděním exchange.</span><span class="sxs-lookup"><span data-stu-id="57609-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="57609-107">Pokud **není doručena jednotlivá výstraha z určitého souboru nebo knihovny**, pokuste se ji odstranit a znovu vytvořit.</span><span class="sxs-lookup"><span data-stu-id="57609-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="57609-108">Viz [Správa, zobrazení nebo odstranění sharepointových výstrah,](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) abyste výstrahu znovu vytvořili.</span><span class="sxs-lookup"><span data-stu-id="57609-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="57609-109">Výstrahy nelze odeslat distribuční skupině.</span><span class="sxs-lookup"><span data-stu-id="57609-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="57609-110">Podporovány jsou pouze skupiny Zabezpečení a O365.</span><span class="sxs-lookup"><span data-stu-id="57609-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="57609-111">Šablony e-mailů s výstrahami nelze přizpůsobit.</span><span class="sxs-lookup"><span data-stu-id="57609-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="57609-112">K jejich dosažení je nutné použít Microsoft Flow nebo SharePoint Designer Workflow.</span><span class="sxs-lookup"><span data-stu-id="57609-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
