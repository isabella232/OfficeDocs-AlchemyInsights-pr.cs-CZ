---
title: Přístup k Centru pro správu SharePointu nebo OneDrivu se nedaří
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824428"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="deb7c-102">Přístup k Centru pro správu SharePointu nebo OneDrivu se nedaří</span><span class="sxs-lookup"><span data-stu-id="deb7c-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="deb7c-103">Pokud je web Centra pro správu SharePointu nebo OneDrivu nedostupný nebo nedostupný, může docházet k dočasnému problému se službou, kdy se uživatelům při přístupu k sharepointovým webům nebo obsahu OneDrivu občas dochází ke zpožděním nebo chybám navigace.</span><span class="sxs-lookup"><span data-stu-id="deb7c-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="deb7c-104">Podívejte se [na řídicí panel Stavu služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) a podívejte se, jestli má vaše organizace vliv.</span><span class="sxs-lookup"><span data-stu-id="deb7c-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="deb7c-105">Globálním správcům a správcům SharePointu je potřeba přiřadit sharepointovou licenci.</span><span class="sxs-lookup"><span data-stu-id="deb7c-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="deb7c-106">Nově vytvořené účty, které mají přiřazenou licenci sharepointové licence nebo roli správce, můžou mít problémy s přístupem k SharePointu, například "přístup odepřen" nebo "uživatel nebyl nalezen".</span><span class="sxs-lookup"><span data-stu-id="deb7c-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="deb7c-107">Dejte prosím synchronizaci napříč našimi systémy minimálně 24 hodin.</span><span class="sxs-lookup"><span data-stu-id="deb7c-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="deb7c-108">Chápeme, že 24 hodin se může zdát jako dlouhá doba.</span><span class="sxs-lookup"><span data-stu-id="deb7c-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="deb7c-109">V mnoha případech už pracujeme na řešení.</span><span class="sxs-lookup"><span data-stu-id="deb7c-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="deb7c-110">Privilegované správy identit[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)uživatelům může být odepřen přístup, pokud je povolené časové okno přístupu velmi malé, viz  [Přístup odepřený účtům PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span><span class="sxs-lookup"><span data-stu-id="deb7c-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>