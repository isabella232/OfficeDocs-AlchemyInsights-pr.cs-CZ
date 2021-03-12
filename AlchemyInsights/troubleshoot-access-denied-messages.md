---
title: Poradce při potížích se zprávami s odepření přístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704887"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="3b392-102">Poradce při potížích se zprávami s odepření přístupu</span><span class="sxs-lookup"><span data-stu-id="3b392-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="3b392-103">Pokud někdo dostal zprávu o odepření přístupu do sdílené složky na SharePointu, mohl správce kolekce webů povolit režim uzamčení oprávnění pro uživatele s omezeným přístupem.</span><span class="sxs-lookup"><span data-stu-id="3b392-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="3b392-104">Vypnutí této funkce:</span><span class="sxs-lookup"><span data-stu-id="3b392-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="3b392-105">Přejděte na web, klikněte na ikonu Nastavení a potom klikněte na **Nastavení webu.**</span><span class="sxs-lookup"><span data-stu-id="3b392-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="3b392-106">V **části Správa kolekce webů** klikněte na funkce kolekce **webů.**</span><span class="sxs-lookup"><span data-stu-id="3b392-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="3b392-107">Vedle režimu uzamčení oprávnění pro uživatele s omezeným **přístupem** klikněte na **Deaktivovat.**</span><span class="sxs-lookup"><span data-stu-id="3b392-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="3b392-108">Zpráva o odepření přístupu se může také zobrazit u sdílených složek, pokud je web publikování.</span><span class="sxs-lookup"><span data-stu-id="3b392-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="3b392-109">Informace najdete v článku [o odepření přístupu ke sdílené složce.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="3b392-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="3b392-110">Pokud se někdo při pokusu o zobrazení žádostí o přístup dostal zprávu o odepření přístupu, musí být uživatel přidaný buď jako správce kolekce webů, nebo jako člen skupiny Vlastníci pro tento web.</span><span class="sxs-lookup"><span data-stu-id="3b392-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="3b392-111">Další informace najdete v článku [o odepření přístupu k seznamu](https://go.microsoft.com/fwlink/?linkid=2004220)žádostí o přístup.</span><span class="sxs-lookup"><span data-stu-id="3b392-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="3b392-112">Pokud se uživateli po odebrání z místní služby Active Directory a potom přidaný zpět zpráva o odepření přístupu, podívejte se na článek o odepření přístupu, když se uživatelský účet synchronizuje s [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="3b392-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

