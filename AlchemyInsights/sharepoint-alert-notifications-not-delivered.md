---
title: Oznámení o upozornění SharePointu Nedoručeno
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751236"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="82ef9-102">Oznámení o upozornění SharePointu Nedoručeno</span><span class="sxs-lookup"><span data-stu-id="82ef9-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="82ef9-103">V e-mailu se podívejte do složky Nevyžádaná pošta, protože někdy můžou být upozornění.</span><span class="sxs-lookup"><span data-stu-id="82ef9-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="82ef9-104">Zjistěte, jestli nejsou **Doručená žádná oznámení** nebo jestli není Doručená **jednotlivá výstraha** od konkrétního souboru nebo knihovny.</span><span class="sxs-lookup"><span data-stu-id="82ef9-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="82ef9-105">Nejsou **Doručená jednotlivá upozornění**: Pokud se nedoručení jednotlivých upozornění z určitého souboru nebo knihovny, můžete se pokusit je odstranit a znovu vytvořit.</span><span class="sxs-lookup"><span data-stu-id="82ef9-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="82ef9-106">Další informace najdete v tématu [Správa, zobrazení nebo odstranění upozornění SharePointu](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="82ef9-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="82ef9-107">Nejsou **doručovány všechny výstrahy**: Pokud nejsou doručovány všechny výstrahy z více souborů nebo knihoven, vyhledejte na [řídicím panelu stavu služeb](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) všechny informační zpravodaje a incidenty, které se můžou vyskytovat v SharePointu nebo Exchange.</span><span class="sxs-lookup"><span data-stu-id="82ef9-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="82ef9-108">Problém může být s možností zobrazování nebo zpoždění v e-mailech na SharePointu.</span><span class="sxs-lookup"><span data-stu-id="82ef9-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="82ef9-109">Bude taky důležité poznamenat, jestli se budou doručovány i jiné e-maily, a pokud ne, problém je asi zpoždění Exchange.</span><span class="sxs-lookup"><span data-stu-id="82ef9-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="82ef9-110">Časté otázky k upozorněním:</span><span class="sxs-lookup"><span data-stu-id="82ef9-110">FAQ on alerts:</span></span>

- <span data-ttu-id="82ef9-111">Není možné odesílat upozornění do distribuční skupiny, podporují se jenom skupiny zabezpečení a O365.</span><span class="sxs-lookup"><span data-stu-id="82ef9-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="82ef9-112">Nemůžete upravovat šablony e-mailů. k dosažení těchto cílů musíte použít pracovní postup Microsoft FLOW nebo SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="82ef9-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="82ef9-113">Příbuzná témata</span><span class="sxs-lookup"><span data-stu-id="82ef9-113">Related Topics</span></span>

<span data-ttu-id="82ef9-114">Chcete vyzkoušet tok Microsoftu v SharePointu Online?</span><span class="sxs-lookup"><span data-stu-id="82ef9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="82ef9-115">Vytvoření toku</span><span class="sxs-lookup"><span data-stu-id="82ef9-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="82ef9-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="82ef9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
