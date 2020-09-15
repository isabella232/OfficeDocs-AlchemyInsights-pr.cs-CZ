---
title: Poradce při potížích s odepřením přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690776"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="3c1f9-102">Poradce při potížích s odepřením přístupu</span><span class="sxs-lookup"><span data-stu-id="3c1f9-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="3c1f9-103">Pokud někdo do sdílené složky v SharePointu obdržel zprávu "Access Denied", mohl správce kolekce webů povolit režim uzamčení oprávnění uživatelů s omezeným přístupem.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="3c1f9-104">Vypnutí této akce:</span><span class="sxs-lookup"><span data-stu-id="3c1f9-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="3c1f9-105">Přejděte na web, klikněte na ikonu nastavení a potom na **Nastavení webu**.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="3c1f9-106">V části **Správa kolekce webů**klikněte na **funkce kolekce webů**.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="3c1f9-107">V **režimu uzamčení s oprávněními uživatele s omezeným přístupem**klikněte na **deaktivovat**.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="3c1f9-108">Pokud se jedná o web publikování, může se u sdílených složek objevit taky zpráva odepření přístupu.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="3c1f9-109">Informace najdete v článku [odepření přístupu při přístupu ke sdílené složce](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="3c1f9-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="3c1f9-110">Pokud někdo při pokusu o zobrazení žádostí o přístup zobrazil zprávu "přístup odepřen", musí být uživatel přidán jako správce kolekce webů nebo člen skupiny Vlastníci webu.</span><span class="sxs-lookup"><span data-stu-id="3c1f9-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="3c1f9-111">Další informace najdete v článku [odepření přístupu k seznamu žádostí o přístup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="3c1f9-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="3c1f9-112">Pokud uživatel obdržel zprávu "Access Denied" po jejich odebrání ze služby Active Directory místně a pak se přidal zpět, přečtěte si článek [odepření přístupu při synchronizaci uživatelského účtu s Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="3c1f9-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

