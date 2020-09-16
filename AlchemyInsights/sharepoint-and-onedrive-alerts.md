---
title: Zpoždění při přijímání upozornění SharePointu a OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727236"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="62a05-102">Zpoždění při přijímání upozornění SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="62a05-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="62a05-103">Nejdřív v e-mailu zkontrolujte nevyžádaná nebo Nevyžádaná pošta.</span><span class="sxs-lookup"><span data-stu-id="62a05-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="62a05-104">Pokud **jsou všechny výstrahy z více souborů nebo knihoven zpožděné**, navštivte [řídicí panel stavu služeb](https://portal.office.com/adminportal/home?ref=/servicehealth) a zkontrolujte, jestli nejsou k dispozici žádné informační zpravodaje nebo události, které se můžou vyskytovat v SharePointu nebo Exchange.</span><span class="sxs-lookup"><span data-stu-id="62a05-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="62a05-105">Problém může být v případě, že se jedná o možnost upozorňování SharePointu nebo zpoždění e-mailů prostřednictvím Exchange.</span><span class="sxs-lookup"><span data-stu-id="62a05-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="62a05-106">Také si všimněte, jestli se dodávají další e-maily – Pokud ne, problém se může projevit zpoždění Exchange.</span><span class="sxs-lookup"><span data-stu-id="62a05-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="62a05-107">Pokud není **doručeno konkrétní upozornění z určitého souboru nebo knihovny**, zkuste ho odstranit a znovu vytvořit.</span><span class="sxs-lookup"><span data-stu-id="62a05-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="62a05-108">Další informace najdete v tématu [Správa, zobrazení nebo odstranění upozornění SharePointu](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="62a05-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="62a05-109">Do distribuční skupiny nelze posílat upozornění.</span><span class="sxs-lookup"><span data-stu-id="62a05-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="62a05-110">Podporují se jenom skupiny Security a O365.</span><span class="sxs-lookup"><span data-stu-id="62a05-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="62a05-111">E-mailové šablony nemůžete přizpůsobit.</span><span class="sxs-lookup"><span data-stu-id="62a05-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="62a05-112">K dosažení těchto cílů musíte použít pracovní postup Microsoft Flow nebo SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="62a05-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
